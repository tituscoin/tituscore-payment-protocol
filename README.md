Tituscore Payment Protocol
=======

## Getting Started

```javascript
var PaymentProtocol = require('bitcore-payment-protocol');

var body = PaymentProtocol.PaymentRequest.decode(rawbody);
var request = new PaymentProtocol().makePaymentRequest(body);

var version = pr.get('payment_details_version');
var pki_type = pr.get('pki_type');
var pki_data = pr.get('pki_data');
var serializedDetails = pr.get('serialized_payment_details');
var signature = pr.get('signature');

// Verify the signature
var verified = request.verify();
```

## License

Code released under [the MIT license](https://github.com/tituscoin/tituscore-payment-protocol/blob/master/LICENSE).

Copyright 2018-2019 Titus Coin Core Developers.
