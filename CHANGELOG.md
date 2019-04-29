# UNRELEASED

# 0.1.7 (April 25, 2019)

* Fix an embarrassingly bad bug in [#241]

# 0.1.6 (April 25, 2019)

* Update coursier, giving an order-of-magnitude performance boost to dependency resolution (especially for deep dependency trees)
* Hotkey revamp [#241]
  * Share implementation across monaco and text cells
  * Added new hotkeys: Delete cell (ctrl-option-D), add cell above (ctrl-option-A), add cell below (ctrl-option-B)
  * Up and Down arrows now transition to neighboring cells if cursor is at start/end of cell text
* Display cell execution time while it is running [#253]
* Fix RuntimeError when using a numpy array. 

[#241]: https://github.com/polynote/polynote/issues/241
[#253]: https://github.com/polynote/polynote/issues/253

# 0.1.5 (April 19, 2019)

* Support for importing Zeppelin notebooks [#185]
  * Just drag and drop your `note.json` onto the tree view. 
  * Notebook creation and URL import are now two separate buttons. 
* Can now click between cells to create a new cell [#235]
* New clear output button - deletes all results/outputs of a notebook from UI and underlying file [#237]
* Fix scrolling behavior for selected cell [#240]

[#185]: https://github.com/polynote/polynote/issues/185
[#235]: https://github.com/polynote/polynote/issues/235
[#237]: https://github.com/polynote/polynote/issues/237
[#240]: https://github.com/polynote/polynote/issues/240

# 0.1.4 (April 16, 2019) 

* Style fixes and tweaks [#219], [#230]
* Fix delegation of failed classloadings [#246]

[#219]: https://github.com/polynote/polynote/pull/219
[#230]: https://github.com/polynote/polynote/pull/230
[#246]: https://github.com/polynote/polynote/pull/246

# 0.1.3 (April 12, 2019)

* Import and Export of Notebooks [#215]
  * New download button in Notebook toolbar downloads the ipynb representation of the notebook
  * Can import ipynb files by drag and drop onto the notebooks sidebar UI
  * Additionaly, can import notebooks directly from another Polynote instance when creating a notebook. 
    Just specify a URL instead of a name for the new notebook. 
    
* UI cleanup [#224]
  * drag borders always visible
  * some fixes for notebook panel view
* Vim mode no longer swallows Shift+Enter [#226]
* Fix bug preventing selection of leftmost tab when notebook panel was collapsed [#228]
* Fix bug causing output doubling [#227]
* Fix bug causing run script to fail when certain values were present in the config file [#232]
* Logging and Error visibility improvements [#218]
  * Kernel Error task message now includes stack trace
  * Log kernel errors to Polynote output instead of just UI. 
  * Run script by default tees logs to file to help debugging later

[#215]: https://github.com/polynote/polynote/issues/215
[#218]: https://github.com/polynote/polynote/issues/218
[#224]: https://github.com/polynote/polynote/pull/224
[#226]: https://github.com/polynote/polynote/pull/226
[#227]: https://github.com/polynote/polynote/issues/227
[#228]: https://github.com/polynote/polynote/issues/228
[#232]: https://github.com/polynote/polynote/pull/232

# 0.1.2 (April 5, 2019)

* Run scripts included in HTML Output [#205]
* Add UI support for warnings
* Warn (rather than error) if eta-expansion fails [#216]
* Collapsible sidebars [#11]
* Cells now show execution progress of top-level statements (scala cells only) [#221]
* Add VIM mode [#220]
* Additional bug fixes and UI tweaks ([#212], [#222])

[#11]:  https://github.com/polynote/polynote/issues/205
[#205]: https://github.com/polynote/polynote/issues/205
[#212]: https://github.com/polynote/polynote/issues/212
[#216]: https://github.com/polynote/polynote/pull/216
[#220]: https://github.com/polynote/polynote/issues/220
[#221]: https://github.com/polynote/polynote/pull/221
[#222]: https://github.com/polynote/polynote/pull/222




# 0.1.1 (April 2, 2019)

* Initial release of Polynote! :) 