Python.sugar
============
The source for a work-in-progress Sugar for the [Espresso text-editor][espresso] for development with [Python][].

[espresso]:	http://macrabbit.com/espresso/	"The Espresso text editor"
[python]:	http://python.org/				"The Python programming language"

**Note**: If you're looking to download the sugar file to use without having to build from source, you want the [other repository][builtrepo].

[builtrepo]: http://github.com/mthjones/python.sugar/ "The Python.sugar project hosted on GitHub"

How to Use
----------
Install any dependencies as outlined below. The instructions to install them should be available by following the links.

Once the dependencies are installed, you must now build the sugar from source in order to use it. 

Download the source in .zip or .tgz format using the [download button](#download_button) **or** clone this project to your computer using git:

	git clone git://github.com/mthjones/python.sugar-source.git/ "PySugar"

Navigate to the folder containing what you just cloned and open the Python.xcodeproj file in Xcode.

	cd PySugar
	open Python.xcodeproj

Build the source (⌘B, or Build->Build), and navigate to the build/Debug directory.

	cd build/Debug/

Now copy or link the file to Espresso's Sugars directory (note that you may need to make this directory first).

	mkdir -p ~/Library/Application\ Support/Espresso/Sugars/
	
	mv Python.sugar ~/Library/Application\ Support/Espresso/Sugars/
	-- or --
	ln -s Python.sugar ~/Library/Application\ Support/Espresso/Sugars/

Dependencies
------------
- [Regex.sugar][regexsugar]

[regexsugar]: http://github.com/elliottcable/Regex.sugar "elliottcable's Regex.sugar on GitHub"

More Information
----------------
This sugar uses the naming conventions as outlined by [elliottcable][] in his [Espresso Sugar Standard][ess]. Due to the fact that this standard is not set in stone and being followed by every sugar developer yet, certain themes/foams haven't been created to work with this naming convention. Therefore they may not highlight the syntax quite as nicely as one would like.

There are a few themes/foams that do work with the [Espresso Sugar Standard][ess], however.

- [Monokaffee][] (my own)
- Most themes on [Coffee House][coffee]

[elliottcable]: http://github.com/elliottcable/ "elltiottcable on GitHub"
[ess]: http://github.com/elliottcable/espresso-sugar-standard/tree/master "elliottcable's Espresso Sugar Standard on GitHub"
[monokaffee]: http://github.com/mthjones/monokaffee/ "mthjones' Monokaffee on GitHub"
[coffee]: http://fileability.net/coffee/ "Coffee House"

Because of the unpredictable nature of Espresso sugars and themes/foams, this sugar may change often, so it is worth watching.

TODO
----
See the [Todo List][todo]

[todo]: http://github.com/mthjones/python.sugar-source/blob/master/TODO.markdown
