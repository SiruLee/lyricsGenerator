# lyricsGenerator
A program that generates lyrics given a song title and exports into PowerPoint slides.

# User Case
1. Input the Korean and the English title of the song to search
2. Check if the lyrics found is correct
3. Modify the lyrics as required
4. Save the lyrics into a txt file
5. Click "Generate" button to generate PowerPoint slides of the lyrics
6. Use the output file accordingly

# Directory
## scripts
contains a main script that generates lyrics and slides files
### genLyrics.py
generates a txt file that contains lyrics of a song.
#### Dependency: 
`api/geminiAPI.py`: calls API to generate lyrics
#### Input
the song title in both Korean and English
#### Output: 
a txt file that contains lyrics of a song divided into parts (e.g. verse, chorus, and bridge)

### genSlides.py
generates a pptx file that contains lyrics of a song.
#### Dependency: 
`python-pptx`: for creating PowerPoint files
#### Input
None
#### Output: 
a pptx file that contains lyrics of a song

## api
contains an API code for LLM (e.g. Gemini, ChatGPT, Llama, etc.)

## gui
contains a code that builds a graphical user interface for the program

## data
contains the output files (lyrics in txt and slides in pptx) of the program