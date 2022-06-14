## Windows issue resolve Node JS

I had faced this while making the build of my app. They says me the process is already busy with that directory. So you can't make it.

```
[Error: EBUSY: resource busy or locked, rmdir 'D:\Awesome Work\Development\layzrgg-back-end\dist'] {
  errno: -4082,
  code: 'EBUSY',
  syscall: 'rmdir',
  path: 'D:\\Awesome Work\\Development\\layzrgg-back-end\\dist'
}
```

I had resolved this issue by using the following steps.

- Press `windows key + R` on your keyboard to open the run command box and type this
  `resmon.exe`

- click `OK` to open resource monitor
- In the monitor, navigate to `CPU` tab
- Under `Associated Handles` in the search box, copy the path to the file or folder in question and paste it in there
- Click on the `search icon`
- You should be able to see all the programs using the file or folder right-click each and end-process
