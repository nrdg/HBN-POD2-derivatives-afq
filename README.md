# About this dataset

## General information

This is a DataLad dataset (id: 7ac3bb0b-a231-4531-afa0-cb59b7c79cb3).

## DataLad datasets and how to use them

This repository is a [DataLad](https://www.datalad.org/) dataset. It provides
fine-grained data access down to the level of individual files, and allows for
tracking future updates. In order to use this repository for data retrieval,
[DataLad](https://www.datalad.org/) is required. It is a free and open source
command line tool, available for all major operating systems, and builds up on
Git and [git-annex](https://git-annex.branchable.com/) to allow sharing,
synchronizing, and version controlling collections of large files.

More information on how to install DataLad and [how to install](http://handbook.datalad.org/en/latest/intro/installation.html)
it can be found in the [DataLad Handbook](https://handbook.datalad.org/en/latest/index.html).

### Get the dataset

A DataLad dataset can be `cloned` by running

```
datalad clone https://github.com/nrdg/HBN-POD2-derivatives-afq.git
```

Once a dataset is cloned, it is a light-weight directory on your local machine.
At this point, it contains only small metadata and information on the identity
of the files in the dataset, but not actual *content* of the (sometimes large)
data files.

### Retrieve dataset content

After cloning a dataset, you can retrieve file contents by running

```
datalad get <path/to/directory/or/file>
```

This command will trigger a download of the files, directories, or subdatasets
you have specified.

### Stay up-to-date

DataLad datasets can be updated. The command `datalad update` will *fetch*
updates and store them on a different branch (by default
`remotes/origin/master`). Running

```
datalad update --merge
```

will *pull* available updates and integrate them in one go.

### Find out what has been done

DataLad datasets contain their history in the ``git log``.  By running ``git
log`` (or a tool that displays Git history) in the dataset or on specific
files, you can find out what has been done to the dataset or to individual
files by whom, and when.
