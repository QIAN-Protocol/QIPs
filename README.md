# QIPs

QIAN Improvement Proposals (QIPs) describe standards for the QIAN platform, including core protocol specifications, client APIs, and contract standards.

## Contributing

 1. Review [QIP-0](QIPS/qip-0.md).
 2. Fork the repository by clicking "Fork" button. Here is [a description](template/git-cmd.md).
 3. Add your QIP to your fork of the repository. There is a [template QIP here](template/qip-X.md).
 4. Submit a Pull Request to QIAN's [QIPs repository](https://github.com/QIAN-Protocol/QIPs/).

Your first PR should be a first draft of the final QIP. It must meet the formatting criteria enforced by the build (largely, correct metadata in the header). An editor will manually review the first PR for a new QIP and assign it a number before merging it. Make sure you include a `discussions-to` header with the URL to a new thread on [forum.qian.finance](https://forum.qian.finance/) where people can discuss the QIP as a whole.

If your QIP requires images, the image files should be included in a subdirectory of the `assets` folder for that QIP as follow: `assets/qip-X` (for qip **X**). When linking to an image in the QIP, use relative links such as `../assets/qip-X/image.png`.

When you believe your QIP is mature and ready to progress past the WIP phase, you should ask to have your issue added to the next governance call where it can be discussed for inclusion in a future platform upgrade. If the community agrees to include it, the QIP editors will update the state of your QIP to 'Approved'.

## QIP Statuses

* **Work in progress (WIP)** - a QIP that is still being developed.
* **Proposed** - a QIP that is ready to be reviewed in a governance call.
* **Approved** - a QIP that has been accepted for implementation by the QIAN community.
* **Implemented** - a QIP that has been released to mainnet.
* **Rejected** - a QIP that has been rejected.

## Validation

QIPs must pass some validation tests.  The QIP repository ensures this by running tests using [html-proofer](https://rubygems.org/gems/html-proofer) and [ips_validator](https://rubygems.org/gems/ips_validator).

It is possible to run the QIP validator locally:
```
gem install ips_validator
ips_validator qip <INPUT_FILES>
```

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
