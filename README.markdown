Install steps
-------------

1. User directory is: /Users/&lt;user&gt;.   &lt;top&gt; is a directory where you like to stash such things.

2. `cd ~/<top>`<br />
`git clone git://github.com/tp-freeforall/macports.git`

3. Edit `/opt/local/etc/macports/sources.conf` to include a line: file:///Users/&lt;user&gt;/&lt;top&gt;/macports

4. _(for MSP430)_  `sudo port install msp430-binutils-tinyos msp430-gcc-tinyos msp430-libc-tinyos`

5. _(for AVR)_     `sudo port install avr-binutils-tinyos avr-gcc-tinyos avr-libc-tinyos avrdude-tinyos`


**Note:** nesc 1.3.3 is in the latest macports so it can be installed by doing `sudo port install nesc`.
However, 1.3.4 is required for mspgcc 4.7 support.   1.3.4 is provided by this macport configuration.


**Changelog:**

* Jul  7, 2012: add nesc 1.3.4
    <br>remove msp430-{binutils,gcc,libc}-tinyos, replace with mainstream versions
* Sep 26, 2011: add nesc 1.3.3
* Jul 31, 2010: add nesc 1.3.2 rc
* Dec  2, 2009: add the mcport for avrdude-tinyos. This is used by IRIS.
* Sep 18, 2009: add the macport for nesc 1.3.1 and fix the binutils for MSP430 and AVR for Snow Leopard. The GCC for AVR does not compile properly yet.
* Dec 29, 2008: add the ports for AVR binutils, gcc and libc. Small tweaks for MSP430.
* Dec 28, 2008: add the ports for MSP430 binutils, gcc and libc.
