# Exporting-Google-Maps-to-HTML-in-Python-3.7
Project of a heatmap using gmaps and Google Maps API and export the output as a HTML file.

This repository became a ideia in my mind when I was working in a project to build a heatmap based on sales in the startup that I work. The Company is called Ecofood and its based in Brazil.

Using gmaps package to make a heatmap using a Google Maps API, I tried to export the output as a HTML file several times but I didn't had success.

After a long research on internet (especially on https://github.com/jupyter-widgets/ipywidgets/pull/2278), I found that the problem could be solved by adding a ' \ ' in a specific function from a script called 'embed.py', which is responsible for storage functions that will be used in embed_minimal_html, a Python package that exports figures like gmaps Google Map into a HTML file.

## Steps

- Import embed_minimal_html to your Python Working Space.

- Find 'embed.py' script inside Python or Anaconda folder in your computer. I'm Anaconda User, so my filepath is: 
'C:\Users\arthur\Anaconda3\Lib\site-packages\ipywidgets'

- Open the script, go to line 241 and add a ' \ ' where the arrow is pointing in the following picture.

![Capturar](https://user-images.githubusercontent.com/45671820/58126277-fdab4580-7be8-11e9-93c0-031a0bafd60e.PNG)

Your script should have one ' \ ' before changes, so you must have two in the end. Easy.

As a part of this repository, I uploaded a Jupyer Notebook where you'll have an example of figure export process to HTML file. In this JB, I've made a heatmap based on total amount of contribution that every city of New York State provided for 2016 elections campaign.

And thats the result 

Enjoy !


