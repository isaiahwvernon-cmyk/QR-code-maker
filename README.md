# QR-code-maker
Simple QR code maker

This is a multi QR code generator with a built-in print layout tool.

At a basic level, it lets you enter multiple name and link pairs. Each pair becomes its own QR code with a label. You can preview all of them, then print them cleanly on a page.

Here’s how it works:

First, you add rows. Each row represents one QR code and includes a title (the name shown above the QR) and a link (what the QR code points to).

When you click “Generate All,” the system goes through each row and checks that:

A title exists
The link is valid (it will automatically add “https://” if missing)

For each valid entry, it uses a QR code library to generate the code and display it in the preview area. At the same time, it captures each QR as an image so it can be used later for printing.

The preview section shows all generated QR codes as individual cards, each with a title and a centered QR code. It also updates a count so you can see how many codes are generated.

When you click “Print All,” it does not print the main page. Instead, it creates a new temporary page that contains only the QR codes and their titles. This avoids common browser issues where printing a full UI results in blank pages or broken layouts.

The print page is formatted specifically for paper:

Clean layout with no UI elements
QR codes arranged in a grid (two per row)
Titles above each code
Proper spacing using real-world units (inches) so it prints consistently

Once that page is created, it automatically opens the print dialog.

In short, this tool takes multiple links, turns them into labeled QR codes, and formats them into a clean, printable sheet without the typical browser printing problems.
