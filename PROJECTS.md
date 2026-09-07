# Practical tools for fieldwork, inspection, and everyday work

I build software around tasks I encounter in geospatial and professional work. The common aim is to reduce manual steps while keeping the underlying information clear and usable.

Signal Audio has a public source repository. The remaining write-ups describe projects in active development whose source and downloads are not published here.

## Signal Audio

**Record audio, turn it into text, and keep the results together.**

Signal Audio is a Windows desktop app for recording computer playback, a microphone, or both, and transcribing the resulting audio locally. Named sessions keep original recordings, transcripts, timestamps, and subtitles together.

It also supports importing existing audio and video files. Transcription uses faster-whisper, with speech models downloaded once and cached for later use. It is another example of how I approach software: solve a recurring task, reduce the number of manual steps, and make the result easy to find and use.

**Built with:** Python and faster-whisper.

**Status:** Public source repository, with Windows release instructions.

[View Signal Audio on GitHub](https://github.com/elliottcromer4-beep/signal-audio)

## FieldNote

**Mobile field collection with a clear route back to GIS.**

Field observations often end up spread across camera rolls, notebooks, and separate mapping applications. FieldNote brings location, geometry, photographs, and attributes into project-based collection sessions.

The current beta includes point, line, and area collection; route recording; layer organisation; photographs and notes; and geometry editing. It supports common exchange formats including GeoJSON, CSV, KML, and zipped Shapefiles, alongside map and report outputs. Device-reported position accuracy is visible so records can be reviewed in context.

A companion project, FieldNote Studio, explores a desktop workspace for survey data, maps, and reporting.

**Built with:** React, TypeScript, Capacitor, Leaflet, and IndexedDB.

**Status:** Beta under active development, with Android and iOS wrappers and a browser build.

## Inspector

**Keep inspection findings connected to the data that supports them.**

Reviewing an asset can involve point clouds, video, drawings, GIS layers, and photographs. The reporting work becomes harder when observations lose their connection to those sources.

Inspector is a desktop workspace for reviewing multiple datasets and recording observations against them. Its workflows include point-cloud annotation, timecoded video evidence, image capture, finding review, and an inspection-report editor with editable Word export. Spatial exports help carry findings back into mapping workflows.

The emphasis is on traceability: moving from a dataset to an observation, supporting evidence, a reviewed finding, and a report.

**Built with:** Python, PySide6, PyVista, GeoPandas, OpenCV, and python-docx.

**Status:** Desktop application under active development.

## Report Studio

**One project dataset for a mooring inspection report and its map.**

Preparing reports and maps separately creates repeated work and opportunities for the outputs to disagree. Report Studio brings the mooring register, line assessments, photographs, and report sections into one local desktop project.

The prototype supports spreadsheet import, geotagged photograph review, line-by-line assessments, report previews, PDF output, interactive HTML maps, and project backups. Review controls help identify photographs that still need position or line confirmation before final export.

Report wording is generated from structured project data, with manual editing and review. The aim is to make recurring reporting more consistent while keeping the professional assessment with the person preparing it.

**Built with:** React, TypeScript, Electron, Leaflet, and IndexedDB.

**Status:** Windows desktop prototype under active development.

## VisionForge

**A desktop workflow from video footage to an object-detection dataset.**

Useful machine-learning work depends on preparing and reviewing data, but frame extraction, labelling, dataset organisation, and training often require several disconnected tools.

VisionForge brings these stages into one project workspace. Its development workflow covers video import, frame extraction and filtering, bounding-box annotation, dataset splits, YOLO training, inference review, and exports in common annotation formats.

This builds on my interest in applying computer vision to real imagery problems, including the vegetation-analysis work described in my [geospatial portfolio](PORTFOLIO.md#uav-vegetation-analysis-and-machine-learning).

**Built with:** React, Electron, Python, FFmpeg, and YOLO tooling.

**Status:** Desktop project under active development.

## WorkTrack

**Simple time capture with reports ready for professional use.**

Accurate time records are useful only if keeping them does not interrupt the work. WorkTrack combines a floating timer with project, client, and task records in a local desktop application.

It includes time-entry review, project summaries, backups, and PDF, Excel, and CSV exports. Reports present hours in both clock and decimal formats, and spreadsheet exports retain numeric values for further analysis.

The aim is to shorten the path from doing the work to producing a clear timesheet.

**Built with:** Python, CustomTkinter, SQLite, ReportLab, and openpyxl.

**Status:** Working desktop application, with ongoing development.

---

[Back to my profile](https://github.com/elliottcromer4-beep) · [Geospatial portfolio](PORTFOLIO.md) · [LinkedIn](https://www.linkedin.com/in/elliott-cromer-a7a9761a7/)
