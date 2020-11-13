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


# QIPs

QIAN改进提案（QIP）描述了QIAN平台的标准，包括核心协议规范，客户端API和合约标准。

## 步骤

 1. 查看[QIP-0](QIPS/qip-0.md)。
 2. 单击“Fork”按钮Fork存储库。查看[说明](template/git-cmd.md)。
 3. 将你的QIP添加到Fork的存储库中。查看此处[QIP模板](template/qip-X.md)。
 4. 提交一个Pull Request到QIAN的QIPs[存储库](https://github.com/QIAN-Protocol/QIPs/)。


你的第一个提案，应该是最终QIP的草案。 它必须满足所需的格式设置标准（主要是报头中的正确元数据） 。编辑者将手动查看新QIP的第一个提案，并在合并前为其分配一个编号。 确保你在[forum.qian.finance](https://forum.qian.finance/)上新帖子的URL中包含一个`discussions-to` 的报头，以便社区用户讨论QIP。

如果你的QIP包含图片，则图片文件应包含在该QIP的`assets` 文件夹的子目录中，如下所示： `assets/qip-X` (for qip **X**)。 链接到QIP中的图像时，请使用相对链接，例如 `../assets/qip-X/image.png`。

当你认为自己的QIP已经成熟, 并且准备好通过WIP阶段时，您需要发起请求,将您的问题添加到下一个治理会议中，以便在讨论将来的平台升级时，将此问题纳入讨论。 如果社区同意，则QIP编辑会将你的QIP状态更新为“已批准”。




## QIP 状态

* **进行中 (WIP)** -仍然处于推进过程中的QIPs。
* **已提交** - 已准备好在治理会议中进行审核的QIPs。
* **已批准** - 已被QIAN社区接受用于实施的QIPs。
* **已实施** - 已发布到主网的QIPs。
* **已驳回** - 已被拒绝的QIPs。


## 验证

QIP必须通过一些验证测试。 QIP 存储库确保通过使用 [html-proofer](https://rubygems.org/gems/html-proofer) 和[ips_validator](https://rubygems.org/gems/ips_validator) 来运行测试。

也可以在本地环境运行QIP验证器：
```
gem install ips_validator
ips_validator qip <INPUT_FILES>
```

## 版权

通过[CC0](https://creativecommons.org/publicdomain/zero/1.0/)放弃版权和相关权利。

