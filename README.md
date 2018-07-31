Fissacoin integration/staging tree
================================

https://www.fissacoin.com

Copyroght (c) 2009-2018 Novacoin Developers<br/>
Copyright (c) 2009-2018 Bitcoin Developers<br/>
Copyright (c) 2011-2018 Litecoin Developers<br/>
Copyright (c) 2017-2018 Fissacoin Developer (Marco Kreef C++ & Joshua Hiwat PHP:PDO)<br/>
Copyright (c) 2017-2018 Fissacoin Designer (Carlo Carels)

Fissacoin
----------------

Fissacoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 2.5 minute block targets
 - ~28 million total coins

The rest is the same as Bitcoin.
 - 50 coins per block
 - 2016 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Fissacoin client sofware, see https://www.fissacoin.com.

License
-------

Fissacoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

What is Fissacoin?
-------------------

It all started with the desire to make paying at an event easier, faster and more secure. Untill now the majority of festivals or events have used plastic coins. In the current digital era such an old-fashioned method is outdated. Our wish was to make it digital. 

Throughout the exploration of the market we stumbled upon many rules and regulations and a conservative approach towards digital transactions with real fiat money. Then we discovered and studied blockchain technology. We consider blockchain technology as safer and more secure and thanks to a more liberal implementation it's ideal for the event industry.

At Fissacoin, our mission is to root out hard plastic coins! 
We are the coolest digital payment system on the planet. We'll setup the greatest global network for party people, with fun and innovative content and experiences. 

At Fissacoin, we get people celebrating. We fuel the even industry conversation. We'll use our reputation not only to make this product work but also to support upcoming events and broaden our network to include a variety of parties as well as a wide range of partners. And of course, developing is at the heart of everything we do. We are the technical insider bringing audiences the safest digital payment service for events

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./fissacoin-qt_test

