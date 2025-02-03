# Developers Guide to Scripted Spin-up of New E-commerce Storefronts

This guide provides a step-by-step tutorial on how to automate the setup of new e-commerce storefronts from a home server using Photon OS, Docker, and a reverse proxy.

[Available on LinkedIn](https://www.linkedin.com/pulse/run-aspnet-ecommerce-platforms-from-home-nopcommerce-virto-weeden-cexaf)

## Table of Contents
1. [Fork Required Repositories](#fork-required-repositories)
2. [Add Repositories as Git Submodules](#add-repositories-as-git-submodules)
3. [Setup Photon VM](#setup-photon-vm)

## Part 1: Fork Required Repositories

To begin, you need to fork the following repositories:

1. [nopSolutions/nopCommerce](https://github.com/nopSolutions/nopCommerce)
2. [VirtoCommerce/vc-platform](https://github.com/VirtoCommerce/vc-platform)
3. [umbraco/Umbraco-CMS](https://github.com/umbraco/Umbraco-CMS)
4. [Kentico/Kentico](https://github.com/Kentico/Kentico)
5. [SiteCore/SiteCore](https://github.com/SiteCore/SiteCore)
6. [grandnode/grandnode](https://github.com/grandnode/grandnode)
7. [simplcommerce/SimplCommerce](https://github.com/simplcommerce/SimplCommerce)

## Part 2: Add Repositories as Git Submodules

Once you have forked the repositories, add each of them as a git submodule to your current repository. Use the following commands:

```pwsh
git submodule add https://github.com/scott-weeden/nopCommerce.git nopCommerce
git submodule add https://github.com/scott-weeden/vc-platform.git vc-platform
git submodule add https://github.com/scott-weeden/Umbraco-CMS.git Umbraco-CMS
git submodule add https://github.com/scott-weeden/Kentico.git Kentico
git submodule add https://github.com/scott-weeden/SiteCore.git SiteCore
git submodule add https://github.com/scott-weeden/grandnode.git grandnode
git submodule add https://github.com/scott-weeden/SimplCommerce.git SimplCommerce
```
## Part 3: Create a nightly build for each platform

| Platform         | Workflow Status Badge                                                                                      |
|------------------|------------------------------------------------------------------------------------------------------------|
| nopCommerce      | ![Workflow Status](https://github.com/scott-weeden/nopCommerce/actions/workflows/NIGHTLY-BUILD/badge.svg)  |
| VirtoCommerce    | ![Workflow Status](https://github.com/scott-weeden/vc-platform/actions/workflows/NIGHTLY-BUILD/badge.svg) |
| Umbraco-CMS      | ![Workflow Status](https://github.com/scott-weeden/Umbraco-CMS/actions/workflows/NIGHTLY-BUILD/badge.svg)       |
| Kentico          | ![Workflow Status](https://github.com/scott-weeden/Kentico/actions/workflows/NIGHTLY-BUILD/badge.svg)           |
| SiteCore         | ![Workflow Status](https://github.com/scott-weeden/SiteCore/actions/workflows/NIGHTLY-BUILD/badge.svg)         |
| GrandNode        | ![Workflow Status](https://github.com/scott-weeden/grandnode/actions/workflows/NIGHTLY-BUILD/badge.svg)       |
| SimplCommerce    | ![Workflow Status](https://github.com/scott-weeden/SimplCommerce/actions/workflows/NIGHTLY-BUILD/badge.svg)|
