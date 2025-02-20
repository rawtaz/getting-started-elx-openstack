<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/github_username/repo_name">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
    <img src="images/terraform.png" alt="Logo" width="80" height="80">
    <img src="images/openstack.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Getting started with Terraform on ELASTX OpenStack</h3>

  <p align="center">
    Infrastructure as Code
    <br />
    <br />
       <a href="https://github.com/elastx/getting-started-elx-openstack/issues">Report Bug</a>
    ·
    <a href="https://github.com/elastx/getting-started-elx-openstack/issues">Request Feature</a>
  </p>
</p>


<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>


<!-- ABOUT THE PROJECT -->
## About The Project

This is a walkthrough from a clean tenant and the point is to use this as a boiler plate for several use-cases. What you will get:

* A network stack
* Bastion host where you can manage your infrastructure
* Web servers spread out over three availability zones with a Load Balancer
* Using terraform remote state to reference resources from earlier step


<!-- GETTING STARTED -->
## Getting Started

The repository is constructed to be used as a starting point, on an empty OpenStack tenant, with the goal to get you started using terraform.
The repository is structured in 4 separated parts. Each can be followed as instructions in order, or more advanced - used individually (with awareness of configuration!)

* [00_Start_here](./00_Start_here/README.md) To generate Keypair
* [01_Router_Networking_Bastion](./01_Router_Networking_Bastion/README.md) To create a router, a network with a subnet and a bastion host
* [02_Web_Servers_LBaaS](./02_Web_Servers_LBaaS/README.md) To setup web-servers and a loadbalancer
* [03_Tear_down](./03_Tear_down/README.md) To clean up the tenant in Openstack

### Prerequisites

* OpenRC file from openstack sourced
* Terraform
* Empty tenant in openstack

In order to use this repository on an existing openstack tenant, you will have to make adjustments in `example.auto.tfvars` to fit your environment of each section.

<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/elastx/getting-started-elx-openstack/issues) for a list of proposed features (and known issues).


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

> We accept PRs for expanding and improve upon these examples


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.


<!-- CONTACT -->
## Contact

Team CS - [Elastx Support](http://support.elastx.se) - support@elastx.se
