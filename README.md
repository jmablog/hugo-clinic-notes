## Hugo Clinic Notes

A Hugo theme for the generation, organisation, and viewing of patient notes written in markdown, ideal for a physiotherapy or similar clinic that needs to maintain patient records.

![](images/screenshot.png)

- View all notes organised by date
- View all patients organised alphabetically
- Jump straight to latest note by date
- Jump straight to last modified note
- Auto generate patient, date, and description metadata from filenames

### Prerequisites

You need to install the Hugo CLI. For macOS users, you can install with [homebrew](https://brew.sh/).
```
brew install hugo
```

For Windows users, you can install with [choco](https://chocolatey.org/):
```
choco install hugo-extended -confirm
```

### Getting started

Create a new Hugo project folder at the command line with 

```
hugo new site your-project-name
```

Then change into that directory and run:

```
cd your-project-name
git submodule add https://github.com/jmablog/hugo-clinic-notes.git themes/hugo-clinic-notes
```

Next, copy the contents of the [`exampleSite/config.toml`](https://github.com/jmablog/hugo-clinic-notes/blob/master/exampleSite/config.toml) to your own project's `config.toml`. You can update the fields found in this file using the comments provided (the lines after `#`) as a guide.

Finally, run:

```
hugo server -F 
```

and open your preferred browser to the localhost address Hugo gives you at the command line to view your notes' homepage.

**If you are seeing a blank page it is probably because you have nothing in your `content/all` directory. Let's add some!**

### Adding patients

TODO