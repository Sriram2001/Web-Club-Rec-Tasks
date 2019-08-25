<h1>Slack Bot To Get Lyrics Of Songs</h1>

<h2>Resources used:</h2>
  <a href="https://www.fullstackpython.com/blog/build-first-slack-bot-python.html">https://www.fullstackpython.com/blog/build-first-slack-bot-python.html</a>
  <a href="https://github.com/Techcatchers/PyLyrics-Extractor">https://github.com/Techcatchers/PyLyrics-Extractor</a>
 
<h2>Instructions for use:</h2>
  Create virtual environment and activate it
  
  Run pip install slackclient==1.3.2 (Any 1.x.x version of slackclient will work fine)
  
  
  Run pip install lyrics-extractor
  
  Create new app in a slack workspace and get 'bot user oauth access token' and replace in starterbot.py
  
  Run export SLACK_BOT_TOKEN='your bot user access token here'
  
  You will need an API Key and Engine ID of Google Custom Search JSON API.

  Create your new Custom Search Engine here to get your Engine ID: https://cse.google.com/cse/create/new

  Add any of the following or all websites as per your choice in your Custom Search Engine:

  https://genius.com/
  http://www.lyricsted.com/
  http://www.lyricsbell.com/
  https://www.glamsham.com/
  http://www.lyricsoff.com/
  http://www.lyricsmint.com/
  
  You are free to customise your Custom Search Engine by prioritising any of your preferred keywords, excluding any web pages or turning on the 'Safe Search' feature.

  NOTE: Please don't turn on the 'Search the entire Web' feature as it is currently not possible to scrape from any random sites appearing in the search results using the pyLicics library.

  Visit here to get your API key: https://developers.google.com/custom-search/v1/overview

  Replace your API key and Search engine ID in starterbot.py
  
  Run python starterbot.py command to start the bot
  
  Create a new channel in slack and add the bot to it
  
  Now whenever you type @<Bot name>lyric: <songname>, the bot will display the lyrics of the song
  
  
