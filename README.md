# TgFolderClone
Telegram bot for using folderclone

## Usage
1. Follow instructions at https://github.com/Spazzlo/folderclone on how to create SA accounts.
2. Copy the .json files to **accounts** folder.
3. Rename `config.py.sample` to `config.py`.
4. Edit the values in `config.py`.
5. Run `py folderclone.py`.

## Usage in telegram bot
`/clone <source_id> <dest_id> <thread> <view>`

`source_id` - Drive ID of the folder you want to copy from. (Required)

`dest_id` - Drive ID of the folder you want to copy into. (Required)

`thread` - Amount of threads to use. The higher the more resource it requires. Default - 10

`view` - 0 - Tree View. 1 - Basic View. Default - Tree View.


### Note
`folderclone.py` - Modified version of `multifolderclone.py` from https://github.com/justcopy/Multifolderclone

<details>
  <summary>Deploying to Heroku</summary>
  
  ## TODO
  To deploy to heroku, open clonerbot.py and change `py folderclone.py` on line `55` to `python3 folderclone.py` and deploy.
  
  (Yes I am too lazy to make a condition for it.)
  
  ## Concerning thread number
  Recommended thread number for heroku is 25.
  
  40 will cause occasional RAM over usage and stall the app.
  
  50 if you want to risk your app hanging.
  
  Anything above 50 will more likely crash the app.
  
</details>
