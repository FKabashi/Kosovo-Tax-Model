
# Kosovo Tax Model

Technical notes, configuration scripts and automation for the Kosovo Tax Model.

## Windows Launcher Configuration

```bat
@echo off
title Kosovo Tax Model

cd /d "%USERPROFILE%\Documents\Models\Kosovo-TE-Models\Kosovo-TE-Models"

"%LOCALAPPDATA%\Programs\R\R-4.5.1\bin\Rscript.exe" --vanilla -e "app <- source('Modules/TaxModelLauncher.R', encoding='UTF-8')$value; shiny::runApp(app, launch.browser=TRUE)"

pause
```

## Purpose

Launch the Kosovo Tax Model directly from the desktop without opening RStudio manually.

## Configuration Date

24 November 2026
