# Constraining the parameters of GW150914 & GW170104 with numerical relativity surrogates

**Prayush Kumar<sup>1</sup>, Jonathan Blackman<sup>2</sup>, Scott E. Field<sup>3</sup>, Mark Scheel<sup>2</sup>, Chad R Galley<sup>4,2</sup>, Michael Boyle<sup>1</sup>, Lawrence E. Kidder<sup>1</sup>, Harald P. Pfeiffer<sup>5</sup>, Bela Szilagyi<sup>2, 4</sup>, Saul A. Teukolsky<sup>1, 2</sup>**

**<sup>1</sup>Cornell Center for Astrophysics and Planetary Science, Cornell University, Ithaca, New York 14853, USA**

**<sup>2</sup>Theoretical Astrophysics, Walter Burke Institute for Theoretical Physics, MC 350-17, California Institute of Technology, Pasadena, CA 91125, USA**

**<sup>3</sup>Department of Mathematics, University of Massachusetts, Dartmouth, MA 02747, USA**

**<sup>4</sup>Jet Propulsion Laboratory, California Institute of Technology, Pasadena, CA 91109, USA**

**<sup>5</sup>Max Planck Institute for Gravitational Physics (Albert Einstein Institute), Am Mühlenberg 1, 14476 Potsdam-Golm, Germany**

## License

![Creative Commons License](https://i.creativecommons.org/l/by-sa/3.0/us/88x31.png "Creative Commons License")

This work is licensed under a [Creative Commons Attribution-ShareAlike 3.0 United States License](http://creativecommons.org/licenses/by-sa/3.0/us/).


## Introduction

This repository provides posterior Samples from the analysis of the first two heavy binary black hole merger events - GW150914 and GW170104 - in [Kumar et al. (2018)](https://arxiv.org/abs/1808.08004). Samples are included for the multimodal numerical relativity surrogate model NRSur7dq2, and the precessing phenomenological model IMRPhenomPv2 (see our paper and references therein for details of these models). Also provided is a Python notebook [**UsingPosteriorSamples.ipynb**](https://github.com/prayush/GW150914_GW170104_NRSur7dq2_Posteriors/blob/master/UsingPosteriorSamples.ipynb) that demonstrates how to read and visualize our posterior proability density files.

We encourage use of these data in scientific work. If you use the material provided here, please cite the paper using the reference:
```
@article{Kumar:2018hml,
      author         = "Kumar, Prayush and Blackman, Jonathan and Field, Scott E.
                        and Scheel, Mark and Galley, Chad R. and Boyle, Michael
                        and Kidder, Lawrence E. and Pfeiffer, Harald P. and
                        Szilagyi, Bela and Teukolsky, Saul A.",
      title          = "{Constraining the parameters of GW150914 \&amp; GW170104
                        with numerical relativity surrogates}",
      year           = "2018",
      eprint         = "1808.08004",
      archivePrefix  = "arXiv",
      primaryClass   = "gr-qc",
      reportNumber   = "LIGO-P1800166",
      SLACcitation   = "%%CITATION = ARXIV:1808.08004;%%"
}
```

The data are stored in the following files:

 1. [**NRSur7dq2HM_RestrictedPriors.dat**]: Samples from the multidimensional posterior distribution estimated using the full multimodal NR surrogate model NRSur7dq2.
 2. [**NRSur7dq2_RestrictedPriors.dat**]: Samples from the multidimensional posterior distribution estimated using the NR surrogate model NRSur7dq2 with only the dominant l = |m| = 2 modes.
 3. [**IMRPhenomPv2_UnRestrictedPriors.dat**]: Samples from the multidimensional posterior distribution estimated using the precessing phenomenological model IMRPhenomPv2.
 4. [**IMRPhenomPv2_RestrictedPriors.dat**]: Samples from the multidimensional posterior distribution estimated using the precessing phenomenological model IMRPhenomPv2. In this analysis, sampling priors are restricted to 1 <= q <= 2 and spin magnitudes < 0.8, in order to emulate the priors for NRSur7dq2.
  
 These files are available for each event in its individual directory.


