# The Germ Line Age Calculator

The following steps are outlined to demonstrate the functionality of
the Germ Line Age Calculator. These steps are to be used with the
Illumina methylation array data sets (450k or EPIC). Specifically, the
steps outlined below assume that beta-values (SWAN normalized) are
available which can be performed with multiple different open source
tools (ChAMP, Minfi, etc.) as well as other software tools (Partek).

Predicted ages are obtained via the call to a `predict_germ_age()` function.

The functoin expects the following arguments:

1. `x` - a numeric matrix of beta values.

```

X23       X28       X33       X47       X52       X34
0.13191   0.20154   0.107196  0.219992  0.109324  0.0830337
0.0394964 0.0288217 0.0502977 0.0289973 0.0499303 0.0345183
0.110789  0.0293556 0.0807749 0.0306088 0.0859292 0.0834235
0.0424816 0.0530358 0.0480805 0.0821266 0.0475171 0.0440236
0.106486  0.136325  0.0739211 0.114175  0.105706  0.109751
0.0468505 0.0410757 0.0406775 0.0277944 0.0375733 0.0484815

```

2. `probeID` - a vector of probe IDs for each row of the `x` matrix.

```

"cg00050873" "cg00212031" "cg00213748" "cg00214611" "cg00455876" "cg01707559"

```

3. `batch` - sentrix barcode numbers for each column of the `x` matrix.

```

1888849019, 1888849019, 1888849020, 1888849020, 1888849035, 1888849094

```

Authors and Contributors
========================

Main author:

Tim Jenkins (tim.jenkins@hsc.utah.edu)

Rewritten by:

Karolis Koncevičius (karolis.koncevicius@gmail.com)

Copyright and License Information
=================================

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

