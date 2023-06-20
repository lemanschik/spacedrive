# Open Source - AwesomeOS powered spacedrive interface
- [ ] Striping the none needed parts
- [ ] Replacing it with opfs.zip and cloud-fs.zip as storage backend and distribution layer
- [ ] Rename jobs to tasks
- [ ] Else keep the layout and UX to have a compatible Interface.
- [ ] Release binarys of it and hire the UI Designer 


## Notes
the usefull entrypoint is in 

```shell
# Main UI 
/interface/app/%24libraryId/index.tsx

# additional keybindings and env meta
/interface/app

# additional packages
/packages/*
```


## Dev Notes
The crap is driven by @tanstack/react-query which is a DoneJS CanJS Observeable Stream clone like million others
How ever this is a great package to shim as adapter as the spacedrive project depends on it for everything under the hood
this is the abstraction layer for all Request Response interactions. 

Sure removing react from the stack also helps but can be done incremental. 

to be compatible we only need the above mentioned package. so we can simple do a spacedrive extension for our explorer. 
project on opfs.zip

