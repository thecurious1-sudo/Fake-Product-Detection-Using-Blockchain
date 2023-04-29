<!-- Other badges-->

![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)
![Ethereum](https://img.shields.io/badge/Ethereum-3C3C3D?style=for-the-badge&logo=Ethereum&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![React Router](https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Web3js](https://img.shields.io/badge/web3.js-F16822?style=for-the-badge&logo=web3.js&logoColor=white)
![Solidity](https://img.shields.io/badge/Solidity-e6e6e6?style=for-the-badge&logo=solidity&logoColor=black)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

<!-- Other badges-->

<br />
<p align="center">
    <img src="https://res.cloudinary.com/dgy8ybeoy/image/upload/v1659287496/favicon_rjjovn.ico" alt="Logo" width="80">
  </a>

  <p align="center">
    Product Authentication System using Blockchain
    <br />
    <a href="https://venerable-crumble-abfbd4.netlify.app/">View Live</a>
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
      </ul>
        <li><a href="#built-with">Built With</a></li>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#running-the-project">Running the project</a></li>
      </ul>
    </li>
    <li><a href="#features">Features</a></li>
    <li><a href="#block-diagram">Block Diagram</a></li>
    <li><a href="#screenshots">Screenshots</a></li>
      <li><a href="#future-scope">Future Scope</a></li>
    <li><a href="#contributors">Contributors</a></li>
  </ol>
</details>

## About The Project

Introducing a decentralized platform for warranty issuance that enables sellers to transfer their warranties to buyers through Polygon-based NFTs. You can now keep your warranties in the digital realm as NFTs, freeing up space in your closet, and ensuring proper ownership proof. Instead of a physical piece of paper, warranties are now in token form. To get started, register below and begin storing your warranties.

Our platform utilizes the Soulbound NFT principle, ensuring that warranties cannot be stolen, with added features such as expiry dates and resell options, making them suitable for various other applications.

## Built With

Following technologies and libraries are used for the development of this website

- [React](https://reactjs.org/)
- [IPFS](https://ipfs.io/)
- [Vercel](https://vercel.com/)
- [React Router](https://reactrouter.com/)
- [Solidity](https://docs.soliditylang.org/)
- [Polygon](https://polygon.technology/)
- [Ethereum](https://ethereum.org/en/)
- [Web3.js](https://web3js.readthedocs.io/)
- [Gelato Ops](https://app.gelato.network/)
- [Tailwind CSS](https://tailwindcss.com/)

## Getting Started

To setup the project locally the steps below.

### Prerequisites

- Please make sure you have [metamask](https://metamask.io/) installed and connected to polygon's mumbai testnet and have some test matic in your wallet

- [Node.js](https://nodejs.org/en/download/)

```sh
  # Homebrew
  brew install nodejs

  # Sudo apt
  sudo apt install nodejs

  # Packman
  pacman -S nodejs

  # Module Install
  dnf module install nodejs:<stream> # stream is the version

  # Windows (chocolaty)
  cinst nodejs.install

```

- [Git](https://git-scm.com/downloads)

```sh
  # Homebrew
  brew install git

  # Sudo apt
  apt-get install git

  # Packman
  pacman -S git

  # Module Install (Fedora)
  dnf install git

```

### Running the project.

The project uses NPM. It is strictly advised to stick with NPM so as to avoid dependency conflicts down the line.

```
## Checkout into the project client directory
cd client

## Install Dependencies
npm install

## Run the Project
npm start

```

Following are the commands to remove/add new dependencies using yarn

```
## Add a new Package
npm install <package-name>

## Remove an existing Package
npm uninstall <package-name>

## Save Package as a Dev Dependency
npm install <package-name> --save-dev
```

## Features

### Issue Warranty

Our platform enables sellers to issue warranties effortlessly by including Order ID, Buyer Wallet Address, and Expiry Date as NFT metadata and issuing it as a Pending Warranty. Additionally, we've employed the Soulbound NFT concept by incorporating the Keccak256 Hash of the Owner ID and Product ID into the NFT metadata. The seller can also monitor all pending, active, and expired warranties issued by them.

### Proof Ownership

When the seller dispatches the warranty to the buyer's dashboard as a Pending Warranty, the buyer must verify their ownership by hashing their wallet address using the Keccak256 hash and comparing it to the hash in the NFT metadata. If the verification is successful, the warranty is minted in the chain and added to the buyer's Active Warranties section on the dashboard, serving as proof of ownership and the warranty until it expires.

### Resell Warranty (UNDER DEVELOPMENT)

Once the warranty is added to the buyer's Active Warranties section, they can transfer ownership in the event of a product resale by inputting the new owner's wallet address. The new owner must then verify their ownership using the same Soulbound hashing method as the previous owner.

### Auto Expiry (UNDER DEVELOPMENT)

If the current time exceeds the expiration time of a product warranty, the Burn Function in the Gelato Ops automatically executes, resulting in the NFT being burned and the warranty being moved to the owner's Expired Warranty section. Although the owner can still use the platform to prove product ownership, they are no longer entitled to warranty benefits.

### Track issued and Expired Warranty

When an owner activates a warranty on their dashboard, the warranty history also displays all of its previous owners, aiding in product ownership and sales tracking.

## Block Diagram

<img src="https://res.cloudinary.com/dgy8ybeoy/image/upload/v1659308834/NFTDocket_aeca19.png" alt="Block Diagram" width="100%">

## Screenshots

Home Page:
<img src="https://res.cloudinary.com/deqgjvwad/image/upload/v1682773271/img1_b5ebuu.png" alt="Logo" width="100%">
Register as Seller Page:
<img src="https://res.cloudinary.com/deqgjvwad/image/upload/v1682776057/img6_hj76hf.png" alt="Logo" width="100%">
Seller Page:
<img src="https://res.cloudinary.com/deqgjvwad/image/upload/v1682773508/img2_evjmfw.png" alt="Logo" width="100%">
Sell Product Page:
<img src="https://res.cloudinary.com/deqgjvwad/image/upload/v1682775872/img5_x9w3zf.png" alt="Logo" width="100%">
Customer Page:
<img src="https://res.cloudinary.com/deqgjvwad/image/upload/v1682773827/img3_thgd8a.png" alt="Logo" width="100%">
Product Page:
<img src="https://res.cloudinary.com/deqgjvwad/image/upload/v1682773974/img4_hrmu3g.png" alt="Logo" width="100%">

## Future Scope

- Implementing this platform in a mobile application could significantly enhance accessibility and versatility.

- Our use of Soulbound NFTs can enable us to issue uniquely certified items, including degrees, tickets, citizenship, and more.

- Introducing gamification on this platform, wherein every issued warranty NFT transfers credits to the seller, which can be redeemed using various schemes, can promote the widespread adoption of the NFT warranty system. These credits can also be utilized as gas fees for sellers issuing NFT warranties, further encouraging businesses to implement this system.

- The implementation of a marketplace can streamline the process, making it truly one-click.

- Our history tracking feature can be used to keep track of sales, particularly for products like cars that frequently change hands.

- With the marketplace in place, we can also introduce the capability of sending the NFT as a notification to the buyer's mobile phone.

## Contributors

Thanks goes to these wonderful people:

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a><img src="https://res.cloudinary.com/deqgjvwad/image/upload/v1682774420/1666774367708_iqcfgv.jpg" width="100px;" alt=""/><br /><sub><b>Vaibhav Jaiswal <br>20ucc126</b></sub></a><br /><a title="Code">💻</a></td>
    <td align="center"><a><img src="https://res.cloudinary.com/deqgjvwad/image/upload/v1682774280/1672312762153_gabuj5.jpg" width="100px;" alt=""/><br /><sub><b>Rudraksh Garg <br> 20ucc124</b></sub></a><br /><a title="Code">💻</a></td>
    <td align="center"><a><img src="https://res.cloudinary.com/deqgjvwad/image/upload/v1682774386/1670846879672_nmoveo.jpg" width="100px;" alt=""/><br /><sub><b>Samarth Dengre <br> 20ucc092</b></sub></a><br /><a title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
