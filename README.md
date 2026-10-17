# gadgets-rembrandt

Rembrandt for the gadgets of [polpo](https://github.com/polpo-system/polpo): a paint program for
Oberon pictures, and the documents that show pictures. With it, `Desktops.OpenDoc` opens .Pict
files and the other picture formats listed in the section Documents of Oberon.Text (gif, xbm, pbm,
pgm, ppm and others, each with its reader package).

```
portia.Install gadgets-rembrandt
```

## Using

    Desktops.OpenDoc Rembrandt.Panel     the tools: pens, colours, selections, flip, rotate, scale
    Desktops.OpenDoc picture.Pict        a picture in a document (RembrandtDocs.Open does the same)

## What is here

    src/Rembrandt0.Mod, Rembrandt.Mod     the picture gadget and its editing
    src/RembrandtDocs.Mod                 picture documents
    src/RembrandtTools.Mod                the tools: flip, rotate, scale, fill, spray and others
    share/Rembrandt.Panel, Rembrandt.Lib  the panel and its icons
    tools/Rembrandt.Tool
    test/RembrandtTest.Mod

The panel lists picture files with gadgets-directories. The sources come from ETH Linux Oberon (OLR, 2017-06-18), converted from Oberon texts to plain
text; the first commit has them unchanged. They compile unchanged with all five of polpo's compilers
(x86, ARM, ARMv7, RISC-V, MIPS).

## Tests

    RembrandtTest.Run      4 checks: a picture gadget made, Default.Pict loaded as a document, the
                           tools loaded, the panel opened; it needs the desktop's display

The license is GPL-3 (`LICENSE`); the code comes from ETH Oberon, whose license (`LICENSE.ETH`)
asks to keep its copyright notice and conditions, which `LICENSE.ETH` does.
