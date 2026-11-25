# predsig: Software for predictive significance testing

**English** · [한국어](README.ko.md)

**Author** Gyeongcheol Cho · [g.cho@psychematrica.org](mailto:g.cho@psychematrica.org)

Version 0.3.0 estimates each predictor’s contribution to prediction in
confirmatory linear regression and reports both coefficient significance and
predictive significance.

## MATLAB

Tested with MATLAB R2026a Update 4 on Windows. Earlier releases have
not been verified.

1. Download [predsig_matlab_0.3.0.mltbx](MATLAB/predsig_matlab_0.3.0.mltbx).
   Open it in MATLAB and choose **Install**.
2. Run `setup_predsig` once to compile the included C engine. If MATLAB needs
   to select a supported compiler, run `mex -setup C` first.
3. Fit the model with `fitlm` and pass it to `predsig.run`. Model fitting
   requires Statistics and Machine Learning Toolbox.

## R

Download [predsig_0.3.0.tar.gz](R/predsig_0.3.0.tar.gz). Install it from the
directory containing the file.

```sh
R CMD INSTALL predsig_0.3.0.tar.gz
```

Installation requires a C toolchain and the `readxl` and `digest` packages.
Fit the model with `lm` and pass it to `predsig::run`.

## Citation and supplementary materials

> Cho, G. (2026). *predsig: Software for predictive significance testing* [Computer software]. https://github.com/PsycheMatrica/predsig/

Report the version used in your analysis. You can obtain this reference from
[`CITATION.cff`](CITATION.cff) or by running `citation("predsig")` in R.
The [paper’s supplementary materials and reproduction code](https://doi.org/10.5281/zenodo.24521729)
are available on Zenodo.

## License

The author’s code and documentation are licensed under CC BY-NC-SA 4.0.
The installers include separate notices for generated and third-party components.
