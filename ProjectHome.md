Simple tool inspired by Ted Mielczarek post:

http://blog.mozilla.com/ted/2009/02/05/command-line-screenshot-tool-for-windows/

One can take a screenshot of a desktop or any window selected by widow title. It is also possible to select rectangle to capture. The result is stored as a png file.

type screenshot-cmd -h to see help.

```
OPTIONS:
	-wt WINDOW_TITLE
			Select window with this title.
			Title must not contain space (" ").
	-wh WINDOW_HANDLE
			Select window by its handle
			(representad as hex string - f.e. "0012079E") 
	-rc LEFT TOP RIGHT BOTTOM
			Crop source. If no WINDOW_TITLE is provided
			(0,0) is left top corner of desktop,
			else if WINDOW_TITLE maches a desktop window
			(0,0) is its top left corner.
	-o FILENAME
			Output file name, if none, the image will be saved
			as "screenshot.png" in the current working directory.
	-h
			Shows this help info.
```