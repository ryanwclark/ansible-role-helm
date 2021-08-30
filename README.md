# Ansible Role: Helm

[![CI](https://github.com/ryanwclark/ansible-role-helm/workflows/CI/badge.svg?event=push)](https://github.com/ryanwclark/ansible-role-helm/actions?query=workflow%3ACI)

This role installs the [Helm](https://helm.sh) binary on any supported host.

## Requirements

N/A

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    helm_version: 'v3.2.1'
    helm_platform: linux
    helm_arch: amd64

Controls for the version of Helm to be installed. See [available Helm releases](https://github.com/helm/helm/releases/). You can upgrade or downgrade versions by changing the `helm_version`.

    helm_bin_path: /usr/local/bin/helm

The location where the Helm binary will be installed.

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - role: ryanwclark.helm




