# APDB

This is a fork of https://gitlab.com/FFP/ffp-apdb-client and https://gitlab.com/FFP/ffp-apdb-server.

## Access Points DataBase (APDB) for Freifunk (Cottbus)
The APDB consists of two parts:
- client side: `apdb-client` (https://github.com/FFCB/apdb-client)
- server side: `apdb-server` (https://github.com/FFCB/ffp-apdb-server)

A productive used installation is available at http://status.freifunk-cottbus.de/

## Installation (at Access Point)
* `ssh` into your AP
* execute the following commands (copy-paste-ready)

```bash
wget -q -O - 'http://status.freifunk-cottbus.de/ffcb-apdb.php' > /etc/init.d/ffcb-apdb && \
chmod +x /etc/init.d/ffcb-apdb; \
/etc/init.d/ffcb-apdb start
```

## Configuration
* edit `/etc/init.d/ffcb-apdb`for your needs

## (Self-)Upgrade
* `ssh` into your AP

```bash
/etc/init.d/ffcb-apdb upgrade
```

## Legal
    APDB is free software: you can redistribute it and/or modify it under the
    terms of the GNU General Public License as published by the Free Software
    Foundation, either version 3 of the License, or (at your option) any later
    version.

    APDB is distributed in the hope that it will be useful, but WITHOUT ANY
    WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
    FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
    details.

    You should have received a copy of the GNU General Public License along with
    APDB. If not, see <http://www.gnu.org/licenses/>.

    Diese Datei ist Teil von APDB.

    APDB ist Freie Software: Sie können es unter den Bedingungen der GNU General
    Public License, wie von der Free Software Foundation, Version 3 der Lizenz
    oder (nach Ihrer Wahl) jeder späteren veröffentlichten Version,
    weiterverbreiten und/oder modifizieren.

    APDB wird in der Hoffnung, dass es nützlich sein wird, aber OHNE JEDE
    GEWÄHRLEISTUNG, bereitgestellt; sogar ohne die implizite Gewährleistung der
    MARKTFÄHIGKEIT oder EIGNUNG FÜR EINEN BESTIMMTEN ZWECK. Siehe die GNU
    General Public License für weitere Details.

    Sie sollten eine Kopie der GNU General Public License zusammen mit diesem
    Programm erhalten haben. Wenn nicht, siehe <http://www.gnu.org/licenses/>.
