# RC24-MailPatch-Portable
A simple, light and portable version of the Mail Patcher for RiiConnect24


## What is this?
This is simply the mailparse.rb file from [this repo](https://github.com/RiiConnect24/RiiConnect24-Mail-Patcher-Windows), but setup with [Travelling Ruby](https://github.com/phusion/traveling-ruby) to provide a simple and easy way to patch your `nwc24msg.cfg` on your own computer under any operating system (Windows, Linux and macOS are supported).

Running the binary will simply patch any `nwc24msg.cfg` in the current directory in-place. That's it. No bloat, no hidden features, just patching.

## How do I use this?
Head to the [Releases](https://github.com/Seriell/RC24-MailPatch-Portable/releases) page, download the file for your OS and extract it to a folder. Then, place your `nwc24msg.cfg` in the same folder and run the binary (`mailparse.exe` on Windows, `./mailparse` in terminal on Linux/macOS)


## Making changes and building releases.
If you make changes to this repo, you can generate new packages with ease.

### You will need (For building, not running)
- Ruby 2.1 (This specific version is needed, I recommend using RVM.
- Bundler
- Rake

Once you have all that, run `rake package` to create all three packages at once.</br>
If you want to make specific packages, specify either `package:linux:x86`, `package:linux:x86_64`, `package:osx` or `package:win32`.

## Credits
- [Phusion](https://github.com/phusion) for [Travelling Ruby](https://github.com/phusion/traveling-ruby).
- [Spotlight](https://github.com/spotlightishere) for creating the original MailParse script.
- [Advanced BAT to EXE Converter](http://www.battoexeconverter.com/) because lets face it, .bat files are ugly.
