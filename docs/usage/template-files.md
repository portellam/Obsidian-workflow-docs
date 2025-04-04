# Template files

## Main Directory
- [Usage](./README.md)

## How does the template file creation work?
My templater plugin configuration uses the `Filename-Template.md` file to choose
what to do with a file when it is created.

Basically, if it is created with a daily or periodic note title type, it will
select the appropriate template and folder:

```txt
{ format: "YYYY-MM-DD", template: "Daily-Notes.md" },
{ format: "GGGG-[W]WW", template: "Weekly-Notes.md" },
{ format: "YYYY-MM", template: "Monthly-Notes.md" },
{ format: "YYYY-[Q]Q", template: "Quarterly-Notes.md" },
{ format: "YYYY", template: "Yearly-Notes.md" },
```

If not, it will just use either the Area template or the default template for the
inbox:

```txt
{ format: "Area", template: "Areas.md" },
{ format: "Default", template: "Untitled.md" },
```

Thanks a lot to `ljavuras` on Github for the [idea][1].

[1]: https://github.com/ljavuras/obsidian-power-tools/tree/main/Filename%20Template