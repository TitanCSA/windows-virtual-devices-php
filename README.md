# Windows-Virtual-Devices PHP SDK

<!-- simple-start:start -->
Use Windows-Virtual-Devices from a PHP app.

**Start here.** Run `composer require titancsa/windows-virtual-devices`, then try the short example below. Install the matching Windows driver separately.
<!-- simple-start:end -->

> [!IMPORTANT]
> **Get the driver without the one-hour demo limit**
>
> On [Discord](https://discord.com/app), choose **Friends → Add Friend**, enter **`titancsa`** and send the project name. Ask about the full **Windows Virtual Devices** driver for this SDK. TitanCSA shares purchase details privately.

`composer require titancsa/windows-virtual-devices`

Windows x64 PHP8.2+; enable FFI extension and `ffi.enable=true`.

```php
require "vendor/autoload.php";
$client=new \TitanCSA\Products\WindowsVirtualDevices\Client();
try {print_r($client->call("status"));} finally {$client->close();}
```

[API and operation schema](docs/API.md). Matching driver installed separately.
