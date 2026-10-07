# Excalidraw PDF Exporter

A simple tool for converting Excalidraw `.svg` files to `.pdf`.

## Instructions
1. Add your `.svg` file to the working directory.
2. Record the width and height fields from the `.svg` using a text editor. 
3. Put these width and height values in `wrapper.html` at the `size`, `width`, and `height` fields.
4. Input your `.svg.` file name at the bottom of `wrapper.html`.
5. Run the following command, making sure to replace `<YOUR_FIGURE>` with your desired `.pdf` figure name (Windows only):
```powershell
& "C:\Program Files\Google\Chrome\Application\chrome.exe" --headless --no-pdf-header-footer --print-to-pdf="$PWD\<YOUR_FIGURE>.pdf" "$PWD\wrapper.html"
```