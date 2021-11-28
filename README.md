# Electronics

## Download
`git clone git@github.com:UCF-Aether/Electronics.git`

OR

`https://github.com/UCF-Aether/Electronics.git`


You don't have to do this if you're using the GitHub Desktop client.

**Initialize submodules:**
`git submodule update --init --recursive`

**Pull changes from submodules:**
`git submodule update --recursive --remote`


## Adding Libraries
1. Create folder under `symbols/`
2. Copy *.dcm and *.lib to new folder
3. Copy *.pretty folder to `footprints/`
4. In KiCAD, Preferences -> Manage Symbol Libraries -> Project Specific
	 Libraries 
5. Click on the plus at the bottom (+)
6. Give name and file path `$KIPRJMOD/symbols/<folder name>/<lib name>.lib`
7. Click on `Migrate Libraries` while the new row is selected
8. Exit; Go to Preferences -> Manage Footprint Libraries -> Project Specific
	 Libraries 
9. Do the same as above but with the path `$KIPRJMOD/footprints/<lib name>.pretty`. You don't have to migrate the library for footprints
