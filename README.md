
## Features
- Lots of integrated SMS APIs.
- Unlimited number of SMSs.
- Faster than most SMS Bomber apps.
- International bombing available.

## Requirements
- Anything which can run Windows, macOS or Linux and has a keyboard on it.
- Python and PIP installed on it.

## Installation and Setup
It's as easy as typing the below commands into your terminal.
```bash
# Clone my repo
git clone https://github.com/amitsharma123234/FuckOff.git

# Move into the work directory.
cd FuckOff

# Install the requirements via PIP.
pip install -r requirements.txt
```

## Options
You can also read this via `python bomber.py -h` or `python bomber.py --help`

```
usage: bomber.py [-h] [--sms SMS] [--threads THREADS] TARGET

positional arguments:
  TARGET                    Target mobile number without country code (default:+91)

optional arguments:
  -h, --help                show this help message and exit
  --sms SMS, -S SMS         Number of sms to target (default: 5000)
  --country COUNTRY, -c COUNTRY
                        Country code without (+) sign (default: 91)
  --threads THREADS, -T THREADS
                            Number of threads (default: 25)
  --proxy, -p           Use proxy for bombing (It is advisable to use this
                          option if you are bombing more than 5000 sms)
  --verbose, -v         Verbose
  --verify, -V          To verify all providers are working or not
```

## Examples
```bash
# The Classic - 25 threads, 50k SMSs, Country Code: +91
python bomber.py <TARGET>

# Classic + Proxy
python bomber.py --proxy <TARGET>
python bomber.py -p <TARGET>

# Here's how you use all possible parameters to your taste.
python bomber.py --proxy --sms 500 --country 91 <TARGET>
python bomber.py -p -S 500 -c 91 -T 30 <TARGET>
```

## Credits and Thanks
- Thanks to Avinash Reddy (https://github.com/AvinashReddy3108/YetAnotherSMSBomber.git)
- Huge kudos to [skp121](https://github.com/skp121) for the original source code. Find it [here](https://github.com/skp121/Sms-Bomber).
- [SpeedX](https://github.com/TheSpeedX)'s [TBomb](https://github.com/TheSpeedX/TBomb) for some API's used here.
