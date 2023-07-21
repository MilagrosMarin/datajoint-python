# Welcome to the DataJoint for Python!

The DataJoint for Python is a framework for scientific workflow management based on 
relational principles. DataJoint is built on the foundation of the relational data 
model and prescribes a consistent method for organizing, populating, computing, and 
querying data.

DataJoint was initially developed in 2009 by Dimitri Yatsenko in Andreas Tolias' Lab at 
Baylor College of Medicine for the distributed processing and management of large 
volumes of data streaming from regular experiments. Starting in 2011, DataJoint has 
been available as an open-source project adopted by other labs and improved through 
contributions from several developers.
Presently, the primary developer of DataJoint open-source software is the company [DataJoint](https://datajoint.com){:target="_blank"}.

## Data Pipeline Example

![pipeline](https://raw.githubusercontent.com/datajoint/datajoint-python/master/images/pipeline.png)

[Yatsenko et al., bioRxiv 2021](https://doi.org/10.1101/2021.03.30.437358){:target="_blank"}

## Installation

- Interactive environment

The environment is configured by [DevContainer] (https://containers.dev/). Here are two options to launch the interactive environment. 

*Please note that to use the DataJoint-Python package with an interactive environment you need a [GitHub](https://github.com/) account.*

     - **Cloud-based Environment: [GitHub Codespaces](https://github.com/features/codespaces)**: 
     This is a highly recommended option for [**tutorial users**](### [Interactive Tutorials](https://github.com/datajoint/datajoint-tutorials){:target="_blank"}). 

     Instructions:
          - Fork the [datajoint-tutorials](https://github.com/datajoint/datajoint-tutorials) repository into your repository.
          - From your `datajoint-tutorials` repository, click on `Code`, then click on `Codespaces` tab, and `+` option will launch the environment by `Create codespace on main` on your fork with default options. *For more control, see the `...` where you may create `New with options...`.*
          - Please be aware that the initial building time for Codespaces may require a few minutes. However, subsequent initiations of Codespaces within your repository will only take a few seconds.
          - *Tip*: Each month, GitHub renews a [free-tier](https://docs.github.com/en/billing/managing-billing-for-github-codespaces/about-billing-for-github-codespaces#monthly-included-storage-and-core-hours-for-personal-accounts) quota of computing and storage. Typically we run into the storage limits before anything else since Codespaces consume storage while stopped. It is best to delete Codespaces when not actively in use and recreate them when needed. We'll soon be creating prebuilds to avoid larger build times. Once any portion of your quota is reached, you will need to wait for it to be reset at the end of your cycle or add billing info to your GitHub account to handle overages.
          - *Tip*: GitHub automatically assigns a name to the codespace, but you have the option to rename it for better identification purposes in the future.

     - **Local Environment**:
     
     We recommend this option for users that after exploring the DataJoint tutorials want to apply the DataJoint-Python for **their own neuroscience experiments** and lab research. Additionally, this option is particularly advantageous for those who have a keen interest in **other modules of the DataJoint-Elements Library** (e.g., Miniscope, DeepLabCut). However, Windows users are recommended to use above option of cloud-based environment since the `s3fs` utility currently limits the access to example data to MacOS and Linux users.

     Instructions:
          - Ensure you have already installed: [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git), [Docker](https://docs.docker.com/get-docker/), [Microsoft's Visual Studio Code (VS Code)](https://code.visualstudio.com/), and [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers). 
          - `git clone` the codebase repository and open it in VSCode
          - Use the `Dev Containers` extension to `Reopen in Container`
          *You will know your environment has finished loading once you either see a terminal open related to `Running postStartCommand` with a final message: `Done`, or the README.md is opened in `Preview`.*
          - Once the environment has launched, please run the following command in the terminal:
          ```
          MYSQL_VER=8.0 docker compose -f docker-compose-db.yaml up --build -d
          ```

- Local development installation

     - Install with Conda

          ```bash
          conda install -c conda-forge datajoint
          ```

     - Install with pip

          ```bash
          pip install datajoint
          ```

For more detailed instructions, see [Quick Start Guide](./quick-start.md).

## Getting Started 

We recommend that you familiarize yourself with the DataJoint interactive tutorials before incorporating DataJoint into your experiments. By completing these tutorials, you will gain hands-on experience in the fundamentals of the DataJoint framework. These acquired skills will enable you to competently design, implement, and manage data pipelines using DataJoint Element in your scientific research efforts.

### [Quick Start Guide](./quick-start.md)

### [Interactive Tutorials](https://github.com/datajoint/datajoint-tutorials){:target="_blank"} on GitHub Codespaces

### [DataJoint Elements](https://datajoint.com/docs/elements/) - Catalog of example pipelines for neuroscience experiments

### Contribute
  - [Development Environment](./develop)

  - [Guidelines](https://datajoint.com/docs/community/contribute/)




