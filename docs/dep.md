# Dépendances
=============

## imagemagick
--------------

Premièrement vous devez vérifier si imagemagick est installé sur votre OS :

```sh
~@root: convert --version
Version: ImageMagick 7.0.0-0 Q16 x64 2015-01-31 http://www.imagemagick.org
Copyright: Copyright (C) 1999-2015 ImageMagick Studio LLC
Features: DPC Modules HDRI OpenMP
Delegates (built-in): bzlib cairo freetype jbig jng jp2 jpeg lcms lqr openexr pangocairo png ps rsvg tiff webp xml zlib
```

Si ce n'est pas le cas, téléchargez le driver http://www.imagemagick.org/download/binaries/ et installez-le.
Vérifiez de nouveau que convert est bien installé.

Si vous exécutez `npm install` et qu'une erreur liée à python est affichée, vérifier que python2.7 est bien installé et exécutez `npm install --python=python27`

Une fois tout installé vous pouvez lancer l'application.