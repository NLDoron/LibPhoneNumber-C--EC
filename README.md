# LibPhoneNumber-CSharp-EC
Version of LibPhoneNumber-C# with external config files

[![Build status](https://ci.appveyor.com/api/projects/status/76abbk0qveot0mbo/branch/master?svg=true)](https://ci.appveyor.com/project/twcclegg/libphonenumber-csharp/branch/master)
[![codecov](https://codecov.io/gh/twcclegg/libphonenumber-csharp/branch/master/graph/badge.svg)](https://codecov.io/gh/twcclegg/libphonenumber-csharp)

# Overview

# libphonenumber-csharp
Original libphonenumber-csharp project is avaibable [here](https://github.com/twcclegg/libphonenumber-csharp).

# From the original WIKI
## Conversion Notes

C# port of Google's [libphonenumber library](https://github.com/googlei18n/libphonenumber).

  The code was rewritten from the Java source mostly unchanged, please refer to the original documentation for sample code and API documentation.

  The original Apache License 2.0 was preserved.

  See [this](https://github.com/twcclegg/libphonenumber-csharp/blob/master/csharp/README.txt "csharp/README.txt") for details about the port.

## Example

```cs
  var phoneNumberUtil = PhoneNumbers.PhoneNumberUtil.GetInstance();
  var e164PhoneNumber = "+44 117 496 0123";
  var nationalPhoneNumber = "2024561111";
  var smsShortNumber = "83835";
  var phoneNumber = phoneNumberUtil.Parse(e164PhoneNumber, null);
  phoneNumber = phoneNumberUtil.Parse(nationalPhoneNumber, "US");
  phoneNumber = phoneNumberUtil.Parse(smsShortNumber, "US");
```

