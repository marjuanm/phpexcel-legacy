<p align="center">
    <img src="https://www.busquedaweb.com/openprojects/phpexcel-legacy/logo.png?v=1" width="auto" height="331" alt="PHPExcel legacy"></a><br>
    <a href="https://github.com/marjuanm/phpexcel-legacy/blob/main/CHANGELOG"><img src="https://www.busquedaweb.com/openprojects/phpexcel-legacy/release.png?v=1" height="20" alt="Release version"></a>
    <a href="https://github.com/marjuanm/phpexcel-legacy/archive/refs/heads/main.zip"><img src="https://www.busquedaweb.com/openprojects/phpexcel-legacy/download.png?v=2" height="20" alt="Download current version"></a>
    <a href="https://github.com/marjuanm/phpexcel-legacy/blob/main/LICENSE"><img src="https://www.busquedaweb.com/openprojects/phpexcel-legacy/license.png" height="20" alt="Project's license"></a>
    <a href="https://software.webxpress.top/projects/phpexcel-legacy/wiki/getting-started/" target="_blank"><img src="https://www.busquedaweb.com/openprojects/phpexcel-legacy/examples.png" height="20" alt="Examples"></a>
</p>

# What is PHPExcel legacy?
**PHPExcel legacy** is a maintenance project for the <a href="https://github.com/PHPOffice/PHPExcel" target="_blank">PHPExcel library</a>. It's important to note, however, that this library is currently **discontinued**; users are encouraged to switch to its successor, **PhpSpreadsheet**.

Nevertheless, I have chosen to maintain and update this library to ensure compatibility with PHP 8+, given that the original PHPExcel only functions with PHP 5 (and similar) versions. The goal of this project is to modernize PHPExcel and gradually complete its migration to PHP 8+.

At present, it's capable of creating basic Excel files in a PHP 8+ environment; however, this has only been tested with older Office formats. It has not been fully tested with modern file formats or current features.

The intention is not to keep the library up-to-date with the latest standards, but rather to provide continuity for legacy applications—specifically those that cannot or do not wish to migrate or rewrite their code, yet still require a way to export data into the Microsoft Excel format.

# 🚀 Updates for the latest version (0.1.0):

This is the initial version of the project; it's based entirely on the source code of the final version of PHPExcel, which was discontinued as of 2015.

# 📋 License:

The legacy version of PHPExcel is distributed under the LGPL 2.1 license—the same license used by PHPExcel—but it's provided "as is." Use it at your own risk; the author assumes no responsibility for data loss, file corruption, hardware damage, loss of profits, or any other consequences resulting from the use of this software.

The software will be updated incrementally as bugs are discovered and the legacy code is tested for compatibility with PHP 8+. We recommend downloading the latest version to minimize the risk of data loss. Always maintain backups of your important data.

# 💻 Installation and examples:

Installing the legacy PHPExcel library is very simple: just download the <a href="https://github.com/marjuanm/phpexcel-legacy/archive/refs/heads/main.zip">latest released version</a>, unzip it, and place the files in the folder where you intend to install the library (for example, `xls`). Then, in the `.php` file from which you will be including the legacy PHPExcel library, add the following:

require("PHPExcel.php");
 
 $cacheMethod = PHPExcel_CachedObjectStorageFactory::cache_in_memory_gzip;
 $cacheSettings = array('memoryCacheSize ' => '256MB');
 PHPExcel_Settings::setCacheStorageMethod($cacheMethod, $cacheSettings);
	      
 $excel = new PHPExcel();

Continue configuring your library just as you did with PHPExcel, as the way it functions is exactly the same. However, it's important to note that errors will **likely** arise when using the full range of legacy PHPExcel functionality in PHP 8+.

These errors will be addressed gradually as they are discovered and the legacy code is tested. **We ask for your patience.**

# ❤️ Donations & community support

If you don’t wish to purchase a commercial license but would like to support this project, thank you very much in advance. You may donate any amount you wish—any contribution is greatly appreciated; please select one of the following methods.

* ⭐ <a href="https://github.com/sponsors/marjuanm?frequency=recurring" target="_blank">GitHub Sponsors</a>
* ☕ <a href="https://ko-fi.com/msproys" target="_blank">Ko-fi</a>
* 💳 <a href="https://www.paypal.com/donate/?business=73JT73SJF2HXY&amount=1&no_recurring=0&item_name=Thank+you+for+donating+and+supporting+PHPExcel+legacy+projects.Many+thanks%21&currency_code=USD" target="_blank">PayPal</a>

We kindly ask you to observe the following guidelines so that we can provide you with the best possible technical support.

* PHPExcel legacy is a project maintained in my spare time.
* Bug reports and feature suggestions are always welcome and will be reviewed as soon as possible.
* Pull requests are always welcome. Well-documented, tested, and high-quality contributions are more likely to be accepted.

# 🤝 Acknowledgments to other projects

The legacy version of PHPExcel is based on PHPExcel; you can find the official repository at the following URL: <a href="https://github.com/PHPOffice/PHPExcel" target="_blank">https://github.com/PHPOffice/PHPExcel</a>. It's currently **archived.**

The PHPExcel development team recommends migrating to <a href="https://github.com/PHPOffice/PhpSpreadsheet" target="_blank">PhpSpreadsheet</a> or another solution.
