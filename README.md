# com.amplexor.imagemap-pdf
------------------------

# Description
**com.amplexor.imagemap-pdf** is a plugin for the [DITA-OT](http://dita-ot.github.io) that extends the **org.dita.pdf2** plugin to manage [DITA imagemap element](https://www.oxygenxml.com/dita/1.3/specs/langRef/base/imagemap.html) in PDF.

Tested on DITA-OT 3.X. with Antenna House 6.6 and 7.x.
Some limitation exists with FOP (tested with FOP 2.4): internal link between image map area and an `@id` on dita content doesn't work.

## Installation
- DITA-OT 3.2 and newer: run `dita --install com.amplexor.imagemap-pdf`
- DITA-OT 3.1 and older: run `dita --install https://github.com/Amplexor/com.amplexor.imagemap-pdf/releases/download/v1.0/com.amplexor.imagemap-pdf-v1.1.zip`

## Parameters
- **imagemap.hotspot.enabled**: set to "yes" to enable imagemap hotspot insertion in the generated PDF.
- **imagemap.hotspot.shape.color**: defines hotspot shape color. The default value is 'blue'.
- **imagemap.hotspot.text.color**: defines hotspot text color. The default value is 'white'.


## Usage with Antenna House
To use this plugin with Antenna House you have to change [pxpi property](https://www.antennahouse.com/product/ahf60/docs/ahf-optset.html#pxpi) in your AHFSettings.xml:
```xml
<formatter-settings pxpi="72"/>
```        

# Warranty
No warranty of any kind is provided. You can however open issues in the [GitHub project]() to report errors, suggest enhancements or evolutions, ask questions.

# Licence
[![license](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0)
