![Preview](https://github.com/sadparadiseinhell/null/blob/main/assets/preview.png)

## Features
- **Dark/Light Theme** changes by pressing the :waning_crescent_moon: button. In the settings you can set your own colors for both themes
- **Weather** displays temperature and description of weather conditions
- **Search** bar opens when you press `S`. To close press `Esc`

## Instructions
### Clone the repo
```
mkdir Git
cd Git
git clone https://github.com/fahimscirex/startpage
```
### Edit location
```
cd startpage/newtab
nano mozilla.cfg
```
replace `%username%` with your username and save the file using `ctrl+o+enter`. Exit Nano using `ctrl+x`
### Copy files of newtab
```
cd
sudo cp -r Git/startpage/newtab/mozilla.cfg /usr/lib/firefox/
sudo cp -r Git/startpage/newtab/local-settings.js /usr/lib/firefox/defaults/pref/
```
### Change Firefox homepage url
Open Firefox>Preference>Home>Homepage and new windows. `file:///home/%username%/Git/startpage/index.html` replace `%username%` with your username and paste the link in custom url box.

## Settings
### Links
To add your own link to your favorite site, you just need to add a line to the HTML code (Index file is named as `index.html`) for example:

```html
<a href="https://www.github.com/">
  <i class="fab fa-github"></i>
</a>
```

### Weather
To display the weather you need to have a free API key, which can be obtained from the [OpenWeatherMap](https://openweathermap.org/api) website.

> If you generated a **new** API key and the weather doesn't work, then try to wait for a while until the key is activated.
