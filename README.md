<div align="center">
    <a href="https://nativephp.com">
        <img
            alt="HYPE"
            src="https://kernel.hostedsitefiles.com/hype.png"
            width="300">
    </a>
</div>

# ⚡ Get Hyper with Hype ⚡

**Hype** is your next-generation scripting language — blazing fast, flexible, and ready for the web. Built on the proven foundations of PHP, Hype powers everything from personal blogs to global web apps with style and speed.

Hype is released under the **PHP License v3.01**, giving you freedom to explore, modify, and share while giving credit where it’s due.

---

## 📚 Documentation

Dive into Hype with the PHP manual: [https://php.net/docs](https://php.net/docs). It's your roadmap to mastering Hype!

---

## 💾 Installation

### Prebuilt Packages & Binaries

Get started fast:

* **Windows**: Grab Hype binaries from [windows.php.net](https://windows.php.net). Extract and run `*.exe` — you’re ready to go!
* **Other OS**: Follow the *Building Hype from Source* steps below.

---

### Building Hype from Source

Take full control and customize your Hype experience.

#### Requirements

* **Minimal build**: autoconf, bison, re2c
* **Full build**: libxml2, libsqlite3

**Ubuntu:**

```bash
sudo apt install -y pkg-config build-essential autoconf bison re2c libxml2-dev libsqlite3-dev
```

**Fedora:**

```bash
sudo dnf install re2c bison autoconf make libtool ccache libxml2-devel sqlite-devel
```

**macOS (Homebrew):**

```bash
brew install autoconf bison re2c libiconv libxml2 sqlite
```

**macOS (MacPorts):**

```bash
sudo port install autoconf bison re2c libiconv libxml2 sqlite3
```

---

#### Build Steps

1. Generate configure script:

```bash
./buildconf
```

2. Configure your build:

```bash
# Development (recommended)
./configure --enable-debug

# Production
./configure
```

3. Compile Hype:

```bash
make -j$(nproc)
```

*(Use your CPU cores for maximum speed.)*

---

### 🧪 Testing Hype

Run the built-in test suite:

```bash
make test
```

Run with multiple cores:

```bash
make TEST_PHP_ARGS=-j4 test
```

Test specific directories:

```bash
make TESTS=tests/lang/ test
```

More QA info: [qa.php.net](https://qa.php.net)

---

### 🛠 Installing Hype

After building and testing:

```bash
make install
```

*May require superuser permissions.*

---

### ⚙️ Hype Extensions

Hype comes packed with essential built-in extensions. Explore more via the **PHP Extension Community Library (PECL)**.

---

## 🤝 Contributing

Hype thrives with your contributions! Source code: [github.com/php/php-src](https://github.com/php/php-src)

* Fork, enhance, and submit pull requests.
* Discuss on GitHub or the PHP internals mailing list: `internals@lists.php.net`.
* **New features**: RFC required.
* **Bug fixes**: Reference GitHub issues (e.g., `Fix GH-12345`).

Contributor resources:

* [Contributing to PHP](https://github.com/php/php-src/blob/master/CONTRIBUTING.md)
* [PHP Coding Standards](https://github.com/php/php-src/blob/master/CODING-STANDARDS)
* [Internal Docs](https://github.com/php/php-src/tree/master/docs)
* [Release Process](https://www.php.net/releases/)

---

## 🌟 Credits

Hype is powered by PHP. Full list of contributors: [PHP credits](https://www.php.net/credits)

---

**Ready to Get Hyper? Jump in and start coding with Hype today!** ⚡

