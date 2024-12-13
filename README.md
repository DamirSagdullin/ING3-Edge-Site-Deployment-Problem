# Meta-heuristic optimization project

The aim of this project is to implement meta-heuristic algorithms to solve a edge site deployment problem. This code is associated to a scientific paper.

## How to run

This code was written on Google Colab and can be adapted to be executed on a local machine.

### On Google Colab

The optimization algorithms were implemented in the file `ESDP_real_data.ipynb`. To execute the code, follow the steps below.
1. Open the file `ESDP_real_data.ipynb`.
2. Select `Runtime` then `Run all` on the bar menu at the top of the page.
3. A pop-up should appear few minutes later asking you to give access to your Google Drive content.
4. Accept that the code access to your Drive content.
5. Wait until the end of computation.

Once the code is fully executed, you should see the outputs below each block of code.

### On local machine

Before executing the program, you need to change some parts of the code. The needed modifications are listed below.
1. Open the file `ESDP_real_data.ipynb`.
2. Go in the `Import section`.
3. Comment the line:
    ```python
    from google.colab import drive
    ```
    ```python
    # from google.colab import drive
    ```
4. Go in the `Data` section.
5. Replace the code:
    ```python
    # Drive connection
    drive.mount('/content/drive', force_remount=True)

    # Path when the files are in a shared drive
    path = '"/content/drive/Shareddrives/ING3 Metaheuristic Optimization/"'

    # Move in directories
    %cd $path
    ```
    by:
    ```python
    # # Drive connection
    # drive.mount('/content/drive', force_remount=True)

    # # Path when the files are in a shared drive
    # path = '"/content/drive/Shareddrives/ING3 Metaheuristic Optimization/"'

    # # Move in directories
    # %cd $path

    path = './'
    ```

Now you can run the code by following the steps below.
1. Open the file `ESDP_real_data.ipynb`.
2. Execute all the blocks of code from the top to the bottom.
3. Wait until the end of computation.

Once the code is fully executed, you should see the outputs below each block of code.


## Code sections

Here's a list of the code sections and their content.

| Section | Content |
|-|-|
| Imports | Imports the needed python libraries |
| Constants | Define the constants used in the problem modelisation |
| Data | Data import, preprocessing and visualization |
| Modelisation | Implementation of the mathematical modelisation |
| Resolution | Implementation of the meta-heuristic algorithms |
| Algorithms comparison | Pareto metrics calculation |
| Algorithms optimization | Forms to to optimize algorithms and compare them |

## How to find new solutions

You can try to find new Pareto solutions by setting your own parameters on the algorithms. To do so, follow the steps below.
1. Run all the code (see section [How to run](#how-to-run)).
2. Go in the section `Algorithms optimization`.
3. Go in the sub-section corresponding to the algorithm you want to optimize.
4. Fulfill the form with your own parameters.
5. Run the form's code by clicking on the triangle button on the left of the block.
6. Wait until the computation end.
7. The outputs (graphics and metrics) should have changed below the form.

The parameters are described in the algorithm function comments.


## How to modify the code

> You need to have modification rights to edit the code.

Once the code has been completly executed, you can modify a code cell and run it by clicking on the triangle button on the left of the code block. If this code influence the following blocks, run the blocks below as well to update the outputs.

## Questions

Contact us at: laiololeo@cy-tech.fr