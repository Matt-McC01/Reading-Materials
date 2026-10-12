# Neuroscience Reading Materials

A collection of reading and Python notebooks for preparing for computational neuroscience school sessions. Start with the maths notebooks, then use the reference documents for topics you want to explore further.

## Suggested study order

| Step | Notebook | Topics |
| --- | --- | --- |
| 1 | [Maths pre-reading](notebooks/Mathematics_for_Neuroscience_pre_read.ipynb) | Differential equations, vectors, and matrices. |
| 2 | [Part 1: Linear algebra](notebooks/Part_1_Linear_Algebra.ipynb) | Vector operations, similarity, basis vectors, and eigenvalues. |
| 3 | [Part 2: Calculus in neuroscience](notebooks/Part_2_Calculus_in_Neuroscience.ipynb) | Differential equations, numerical methods, and neuron and population models. |
| 4 | [Part 3: Stochastic processes](notebooks/Part_3_Stochastic_Processes.ipynb) | Noisy neuron models, stochastic differential equations, and Euler-Maruyama simulation. |

You can preview notebooks on GitHub. To change parameters or run the exercises, open them in Jupyter.

## Run the notebooks locally

You will need Python 3. From the repository's root folder, create a virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python -m jupyter lab
```

On macOS or Linux, activate the environment with `source .venv/bin/activate` instead.

Open a notebook from `notebooks/`, select the Python kernel from your environment, and run its cells in order. Try changing a parameter and comparing the plots to see how the model responds.

The dependency list is based on the notebook imports. Package versions are not pinned, and a full notebook execution has not been verified in this cleanup.

### A couple of notebook details

- The maths pre-reading notebook loads `pixel_matrix.npy` for an image exercise. That file is not included; obtain it separately and place it in `notebooks/`, or skip the image exercise.
- Some pre-reading cells deliberately demonstrate invalid matrix operations. Those cells are expected to raise errors.
- External images need internet access. Existing notebook outputs may come from an earlier run.

## Reference documents

The original filenames are kept inside `references/` so the source material is easy to recognise.

### Maths and programming

- [Maths for neuroscience students](references/mathematics_for_neuroscience_students.pdf)
- [Math tools](references/MathTools.pdf)
- [Summer school maths slides](references/CN3-summer-school-maths-fullslides.pdf)
- [MATLAB for neuroscientists](references/matlab-for-neuroscientists.pdf)

### Neuron models and neural data

- [Biophysical neuronal models](references/Biophysical%20Neuronal%20Models.pdf)
- [Models of simple spiking neurons](references/Models%20of%20Simple%20Spiking%20Neurons.pdf)
- [Wrangling spike trains: Chapter 3](references/Neural_Data_Science_A_Primer_Chapter3_Wrangling_Spike_Trains.pdf)
- [Analog signals: Chapter 5](references/Neural_Data_Science_A_Primer_Chapter5_Analog_Signals.pdf)

### EEG and MEG

- [Fundamentals of EEG measurements](references/Fundamentals%20of%20EEG%20measurements.pdf)
- [The fundamental neural mechanisms of EEG](references/Schaul1998_The%20fundamental%20neural%20mechanisms%20of%20EEG.pdf)
- [Magnetoencephalography: physics, techniques, and applications](references/kim-davis-2021-magnetoencephalography-physics-techniques-and-applications-in-the-basic-and-clinical-neurosciences.pdf)

The [reading list document](references/Reading%20List.docx) is also available.

## Folder layout

```text
notebooks/          Python study notebooks
references/         PDFs and the reading list document
requirements.txt    Python packages used by the notebooks
README.md           Setup, study order, and document index
```

## Credits

The maths pre-reading notebook credits Barry Dillon and notes by Áine Byrne and Rachel Nicks. The reference documents retain their original authorship and notices; this collection does not add a new licence to those materials.

When adding a resource, put it in the appropriate folder, add a link here, and keep its title and author information.
