<div align="center">
  <h1>Medical Image Segmentation Mask Review Tool</h1>
  <p>This project provides an automated tool for reviewing and verifying segmentation masks used for AI training in medical imaging. It checks for data consistency, mask presence, and volume information. The tool updates a reference Excel file and generates detailed comparison reports.</p>

  [<img src="https://img.shields.io/badge/-readme.md-important?style=flat&logo=google-chrome&logoColor=white" />]() [<img src="https://img.shields.io/badge/-tech blog-blue?style=flat&logo=google-chrome&logoColor=white" />]() [<img src="https://img.shields.io/badge/release-v0.0.1-ㅎㄱㄷ두?style=flat&logo=google-chrome&logoColor=white" />]() 
<br/> [<img src="https://img.shields.io/badge/프로젝트 기간2025.01.06 ~ 2025.01.08-fab2ac?style=flat&logo=&logoColor=white" />]()
  

  ![](../header.png)
</div>


## Installation

### OS X & Linux:
```bash
pip install -r requirements.txt
```

### Windows:
```bash
pip install -r requirements.txt
```

Dependencies are listed in the `requirements.txt` file, including:

```
et_xmlfile==2.0.0
nibabel==5.3.2
numpy==2.2.1
openpyxl==3.1.5
packaging==24.2
pandas==2.2.3
python-dateutil==2.9.0.post0
pytz==2024.2
six==1.17.0
typing_extensions==4.12.2
tzdata==2024.2
```

Ensure you have Python 3.8 or newer installed.

## Usage Example

1. Place your `.nii.gz` medical image files in the `img` folder.
2. Place segmentation masks in the `mask` folder, each inside a subfolder named by the corresponding case ID.
3. Ensure a reference Excel file `data.xlsx` is present.
4. Run the script:

```bash
python AI_data_checker.py
```

This will process the data, update `data.xlsx`, and generate `volume_analysis_results.xlsx` with detailed reports.

More examples and usage details are available in the [Wiki][wiki].

## Development Setup

Install all development dependencies and run tests:

```bash
make install
npm test
```

## Release History

* 1.0.0
    * Initial release with core features for mask verification and volume analysis

## Meta

Soyoung Lim  – syl942511@gmail.com

Distributed under the MIT license. See `LICENSE` for more information.

[https://github.com/imsso-bmed/AI_mask_checker](https://github.com/imsso-bmed/AI_mask_checker)

## Contributing

1. Fork the repository (<https://github.com/imsso-bmed/AI_mask_checker/fork>).
2. Create a new branch (`git checkout -b feature/fooBar`).
3. Commit your changes (`git commit -am 'Add some fooBar'`).
4. Push to the branch (`git push origin feature/fooBar`).
5. Create a new Pull Request.

<!-- Markdown link & img dfn's -->
[npm-image]: https://img.shields.io/npm/v/datadog-metrics.svg?style=flat-square
[npm-url]: https://npmjs.org/package/datadog-metrics
[npm-downloads]: https://img.shields.io/npm/dm/datadog-metrics.svg?style=flat-square
[travis-image]: https://img.shields.io/travis/dbader/node-datadog-metrics/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/dbader/node-datadog-metrics
[wiki]: https://github.com/imsso-bmed/AI_mask_checker/wiki

