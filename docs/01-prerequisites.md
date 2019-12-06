# Prerequisites

## Amazon Web Services

This tutorial leverages [Amazon Web Services](https://aws.amazon.com/) to streamline provisioning of the compute infrastructure required to bootstrap a Kubernetes cluster from the ground up.

## Google Cloud Platform SDK

### Install the Google Cloud SDK

Follow the AWS [documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html) to install and configure the `aws` command line utility.

### Set a Default Compute Region and Zone

This tutorial assumes a default region and credentials have been configured.

If you are using the `aws` command-line tool for the first time, please see the AWS [documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html) to get started.

## Running Commands in Parallel with tmux

[tmux](https://github.com/tmux/tmux/wiki) can be used to run commands on multiple compute instances at the same time. Labs in this tutorial may require running the same commands across multiple compute instances, in those cases consider using tmux and splitting a window into multiple panes with synchronize-panes enabled to speed up the provisioning process.

> The use of tmux is optional and not required to complete this tutorial.

![tmux screenshot](images/tmux-screenshot.png)

> Enable synchronize-panes by pressing `ctrl+b` followed by `shift+:`. Next type `set synchronize-panes on` at the prompt. To disable synchronization: `set synchronize-panes off`.

Next: [Installing the Client Tools](02-client-tools.md)
