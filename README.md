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

Fissacoin is a cryptocurrency specially created for music events. Imagine, you're at an event and you want to get something to drink. Up till now festival coins didn’t resemble the worth of the drink, which can be annoying. With Fissacoin that is going to change. From this day forward you will buy your drinks at the price that it's worth. Furthermore we’ve added interchangeability so it will be possible to use Fissacoin on every event. Transactions made in Fissacoin are without fees (i.e. transaction costs) and VAT (value added tax)

Fissacoin is part of Wlove. Wlove is a global operating Dutch producer, concept developer and promoter of international artists and event concepts. Wlove produces international in- and outdoor events such as festivals, stadium shows and world tours. 

Wlove-produced events include URBAN MUSIC FESTIVAL (Netherlands and Belgium), SOIXANTE-NEUF (Netherlands, Spain, United Arab Emirates, Suriname and Sweden), LATIN RUSH (Netherlands), HOLIDAY JAM (Netherlands) and the #1 URBAN event FUTURE URBAN LEGENDS during the Amsterdam Dance Event (ADE) (October 17th to the 21st, 2018) These events accommodate over 150,000 fans worldwide every year. 

Some of the live music concerts Wlove produced or co-produced are from multi-platinum award-winning international artists like Dru Hill, Rick Ross, French Montana, P-Square, Sean Paul, Trey Songz, Miguel, Ciara, Chris Brown, Next, Joe, Jagged Edge, Lloyd, Tyga, Omarion, Pleasure P, Music Soulchild, Dennis Ferrer, Calisway district, Ginuwine, Bow Wow, Jeremih, Salt-n-Pepa, Blackstreet , David Guetta, Steve Angelo, Hippie, Mardi Grass, Elite Moskow, Akon, Ne-Yo and Busta Rhymes.

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

