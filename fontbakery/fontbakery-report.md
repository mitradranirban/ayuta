## FontBakery report

fontbakery version: 0.12.10



## Experimental checks

These won't break the CI job for now, but will become effective after some time if nobody raises any concern.


<details><summary>[1] ayuta[wght].ttf</summary>
<div>
<details>
    <summary>🔥 <b>FAIL</b> Checking that the typoAscender exceeds the yMax of the /Agrave. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/universal.metrics.html#"></a></summary>
    <div>







* 🔥 **FAIL** <p>OS/2.sTypoAscender value should be greater than 1857, but got 1638 instead</p>
 [code: typoAscender]



</div>
</details>
</div>
</details>




## All other checks



<details><summary>[18] ayuta[wght].ttf</summary>
<div>
<details>
    <summary>🔥 <b>FAIL</b> Checking correctness of monospaced metadata. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/opentype.name.html#"></a></summary>
    <div>







* 🔥 **FAIL** <p>The PANOSE numbers are incorrect for a monospaced font.</p>
 [code: mono-bad-panose]



* 🔥 **FAIL** <p>On monospaced fonts, the value of post.isFixedPitch must be set to a non-zero value (meaning 'fixed width monospaced'), but got 0 instead.</p>
 [code: mono-bad-post-isFixedPitch]



* ⚠️ **WARN** <p>The OpenType spec recommends at <a href="https://learn.microsoft.com/en-us/typography/opentype/spec/recom#hhea-table">https://learn.microsoft.com/en-us/typography/opentype/spec/recom#hhea-table</a> that hhea.numberOfHMetrics be set to 3 but this font has 1 instead.
Please read <a href="https://github.com/fonttools/fonttools/issues/3014">https://github.com/fonttools/fonttools/issues/3014</a> to decide whether this makes sense for your font.</p>
 [code: bad-numberOfHMetrics]



</div>
</details>

<details>
    <summary>🔥 <b>FAIL</b> Validates that when an instance record is included for the default instance, its subfamilyNameID value is set to a name ID whose string is equal to the string of either name ID 2 or 17, and its postScriptNameID value is set to a name ID whose string is equal to the string of name ID 6. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/opentype.fvar.html#"></a></summary>
    <div>







* 🔥 **FAIL** <p>'Regular' instance has the same coordinates as the default instance; its subfamily name should be 'regular'.</p>
<p>Note: It is alternatively possible that Name ID 17 is incorrect, and should be set to the default instance subfamily name, 'Regular', rather than ''regular''. If the default instance is 'Regular', NameID 17 is probably the problem.</p>
 [code: invalid-default-instance-subfamily-name]



* 🔥 **FAIL** <p>'Regular' instance has the same coordinates as the default instance; its postscript name should be 'ayuta-regular', instead of 'ayuta-Regular'.</p>
 [code: invalid-default-instance-postscript-name]



</div>
</details>

<details>
    <summary>🔥 <b>FAIL</b> Shapes languages in all GF glyphsets. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/googlefonts.glyphset.html#"></a></summary>
    <div>







* 🔥 **FAIL** <p>GF_Latin_Core glyphset:</p>
<table>
<thead>
<tr>
<th align="left">Language</th>
<th align="left">FAIL messages</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">de_Latn (German)</td>
<td align="left">Some base glyphs were missing: ẞ</td>
</tr>
<tr>
<td align="left">^</td>
<td align="left">Shaper produced a .notdef</td>
</tr>
</tbody>
</table>
 [code: failed-language-shaping]



* ⚠️ **WARN** <p>GF_Latin_Core glyphset:</p>
<table>
<thead>
<tr>
<th align="left">Language</th>
<th align="left">WARN messages</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">de_Latn (German)</td>
<td align="left">Some auxiliary glyphs were missing: ẞ</td>
</tr>
</tbody>
</table>
 [code: warning-language-shaping]



</div>
</details>

<details>
    <summary>🔥 <b>FAIL</b> Check family name for GF Guide compliance. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/googlefonts.name.html#"></a></summary>
    <div>







* 🔥 **FAIL** <p>&quot;ayuta&quot; doesn't start with an uppercase letter.</p>
 [code: starts-with-not-uppercase]



</div>
</details>

<details>
    <summary>🔥 <b>FAIL</b> Check font follows the Google Fonts CJK vertical metric schema <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/googlefonts.vmetrics.html#"></a></summary>
    <div>







* 🔥 **FAIL** <p>OS/2.sTypoAscender is &quot;1638&quot; it should be 1802</p>
 [code: bad-OS/2.sTypoAscender]



* 🔥 **FAIL** <p>OS/2.sTypoDescender is &quot;-410&quot; it should be -246</p>
 [code: bad-OS/2.sTypoDescender]



</div>
</details>

<details>
    <summary>🔥 <b>FAIL</b> Check font names are correct <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/googlefonts.name.html#"></a></summary>
    <div>







* 🔥 **FAIL** <p>Font names are incorrect:</p>
<table>
<thead>
<tr>
<th align="left">nameID</th>
<th align="left">current</th>
<th align="left">expected</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Family Name</td>
<td align="left">ayuta</td>
<td align="left">ayuta</td>
</tr>
<tr>
<td align="left">Subfamily Name</td>
<td align="left">Regular</td>
<td align="left">Regular</td>
</tr>
<tr>
<td align="left">Full Name</td>
<td align="left"><strong>ayuta regular</strong></td>
<td align="left"><strong>ayuta Regular</strong></td>
</tr>
<tr>
<td align="left">Postscript Name</td>
<td align="left"><strong>ayuta-regular</strong></td>
<td align="left"><strong>ayuta-Regular</strong></td>
</tr>
<tr>
<td align="left">Typographic Family Name</td>
<td align="left"><strong>ayuta</strong></td>
<td align="left"><strong>N/A</strong></td>
</tr>
<tr>
<td align="left">Typographic Subfamily Name</td>
<td align="left"><strong>regular</strong></td>
<td align="left"><strong>N/A</strong></td>
</tr>
</tbody>
</table>
 [code: bad-names]



</div>
</details>

<details>
    <summary>🔥 <b>FAIL</b> Check Google Fonts glyph coverage. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/googlefonts.glyphset.html#"></a></summary>
    <div>







* 🔥 **FAIL** <p>Missing required codepoints:</p>
<pre><code>- 0x1E80 (LATIN CAPITAL LETTER W WITH GRAVE)


- 0x1E81 (LATIN SMALL LETTER W WITH GRAVE)


- 0x1E82 (LATIN CAPITAL LETTER W WITH ACUTE)


- 0x1E83 (LATIN SMALL LETTER W WITH ACUTE)


- 0x1E84 (LATIN CAPITAL LETTER W WITH DIAERESIS)


- 0x1E85 (LATIN SMALL LETTER W WITH DIAERESIS)


- 0x1E9E (LATIN CAPITAL LETTER SHARP S)


- 0x1EF2 (LATIN CAPITAL LETTER Y WITH GRAVE)


- 0x1EF3 (LATIN SMALL LETTER Y WITH GRAVE)


- 0x2013 (EN DASH)


- 0x2014 (EM DASH)


- 0x2018 (LEFT SINGLE QUOTATION MARK)


- 0x2019 (RIGHT SINGLE QUOTATION MARK)


- 0x201A (SINGLE LOW-9 QUOTATION MARK)


- 0x201C (LEFT DOUBLE QUOTATION MARK)


- 0x201D (RIGHT DOUBLE QUOTATION MARK)


- 0x201E (DOUBLE LOW-9 QUOTATION MARK)


- 0x2022 (BULLET)


- 0x2026 (HORIZONTAL ELLIPSIS)


- 0x2039 (SINGLE LEFT-POINTING ANGLE QUOTATION MARK)


- 0x203A (SINGLE RIGHT-POINTING ANGLE QUOTATION MARK)


- 0x20AC (EURO SIGN)


- 0x2122 (TRADE MARK SIGN)


- 0x2212 (MINUS SIGN)
</code></pre>
 [code: missing-codepoints]



</div>
</details>

<details>
    <summary>⚠️ <b>WARN</b> Check mark characters are in GDEF mark glyph class. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/opentype.gdef.html#"></a></summary>
    <div>







* ⚠️ **WARN** <p>The following mark characters could be in the GDEF mark glyph class:
acutecomb (U+0301), dotbelowcomb (U+0323), gravecomb (U+0300), tildecomb (U+0303), uni0302 (U+0302), uni0304 (U+0304), uni0306 (U+0306), uni0307 (U+0307), uni0308 (U+0308), uni030A (U+030A), uni030B (U+030B), uni030C (U+030C), uni0326 (U+0326), uni0327 (U+0327), uni0328 (U+0328) and uni0331 (U+0331)</p>
 [code: mark-chars]



</div>
</details>

<details>
    <summary>⚠️ <b>WARN</b> Does GPOS table have kerning information? This check skips monospaced fonts as defined by post.isFixedPitch value <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/opentype.gpos.html#"></a></summary>
    <div>







* ⚠️ **WARN** <p>GPOS table lacks kerning information.</p>
 [code: lacks-kern-info]



</div>
</details>

<details>
    <summary>⚠️ <b>WARN</b> Check accent of Lcaron, dcaron, lcaron, tcaron <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/universal.html#"></a></summary>
    <div>









* ⚠️ **WARN** <p>Lcaron is decomposed and therefore could not be checked. Please check manually.</p>
 [code: decomposed-outline]



* ⚠️ **WARN** <p>dcaron is decomposed and therefore could not be checked. Please check manually.</p>
 [code: decomposed-outline]



* ⚠️ **WARN** <p>lcaron is decomposed and therefore could not be checked. Please check manually.</p>
 [code: decomposed-outline]



* ⚠️ **WARN** <p>tcaron is decomposed and therefore could not be checked. Please check manually.</p>
 [code: decomposed-outline]



</div>
</details>

<details>
    <summary>⚠️ <b>WARN</b> Does the font contain chws and vchw features? <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/universal.html#"></a></summary>
    <div>







* ⚠️ **WARN** <p>chws feature not found in font. Use chws_tool (<a href="https://github.com/googlefonts/chws_tool">https://github.com/googlefonts/chws_tool</a>) to add it.</p>
 [code: missing-chws-feature]



* ⚠️ **WARN** <p>vchw feature not found in font. Use chws_tool (<a href="https://github.com/googlefonts/chws_tool">https://github.com/googlefonts/chws_tool</a>) to add it.</p>
 [code: missing-vchw-feature]



</div>
</details>

<details>
    <summary>⚠️ <b>WARN</b> Font has **proper** whitespace glyph names? <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/universal.glyphnames.html#"></a></summary>
    <div>







* ⚠️ **WARN** <p>Glyph 0x00A0 is called &quot;nbspace&quot;: Change to &quot;uni00A0&quot;</p>
 [code: not-recommended-00a0]



</div>
</details>

<details>
    <summary>⚠️ <b>WARN</b> Validate size, and resolution of article images, and ensure article page has minimum length and includes visual assets. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/googlefonts.article.html#"></a></summary>
    <div>







* ⚠️ **WARN** <p>Family metadata at fonts/variable does not have an article.</p>
 [code: lacks-article]



</div>
</details>

<details>
    <summary>⚠️ <b>WARN</b> Check for codepoints not covered by METADATA subsets. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/googlefonts.subsets.html#"></a></summary>
    <div>







* ⚠️ **WARN** <p>The following codepoints supported by the font are not covered by
any subsets defined in the font's metadata file, and will never
be served. You can solve this by either manually adding additional
subset declarations to METADATA.pb, or by editing the glyphset
definitions.</p>
<ul>
<li>U+02D8 BREVE: try adding one of: yi, canadian-aboriginal</li>
<li>U+02D9 DOT ABOVE: try adding one of: yi, canadian-aboriginal</li>
<li>U+02DB OGONEK: try adding one of: yi, canadian-aboriginal</li>
<li>U+0302 COMBINING CIRCUMFLEX ACCENT: try adding one of: math, cherokee, coptic, tifinagh</li>
<li>U+0306 COMBINING BREVE: try adding one of: old-permic, tifinagh</li>
<li>U+0307 COMBINING DOT ABOVE: try adding one of: syriac, old-permic, canadian-aboriginal, hebrew, malayalam, coptic, tai-le, math, tifinagh, todhri, duployan</li>
<li>U+030A COMBINING RING ABOVE: try adding one of: syriac, duployan</li>
<li>U+030B COMBINING DOUBLE ACUTE ACCENT: try adding one of: osage, cherokee</li>
<li>U+030C COMBINING CARON: try adding one of: tai-le, cherokee</li>
<li>U+0326 COMBINING COMMA BELOW: try adding math</li>
<li>U+0327 COMBINING CEDILLA: try adding math</li>
<li>U+0328 COMBINING OGONEK: not included in any glyphset definition</li>
<li>U+0331 COMBINING MACRON BELOW: try adding one of: sunuwar, thai, syriac, gothic, cherokee, caucasian-albanian, tifinagh</li>
<li>U+1100 HANGUL CHOSEONG KIYEOK: not included in any glyphset definition</li>
<li>U+1101 HANGUL CHOSEONG SSANGKIYEOK: not included in any glyphset definition</li>
<li>U+1102 HANGUL CHOSEONG NIEUN: not included in any glyphset definition</li>
<li>U+1103 HANGUL CHOSEONG TIKEUT: not included in any glyphset definition</li>
<li>U+1104 HANGUL CHOSEONG SSANGTIKEUT: not included in any glyphset definition</li>
<li>U+1105 HANGUL CHOSEONG RIEUL: not included in any glyphset definition</li>
<li>U+1106 HANGUL CHOSEONG MIEUM: not included in any glyphset definition</li>
<li>U+1107 HANGUL CHOSEONG PIEUP: not included in any glyphset definition</li>
<li>U+1108 HANGUL CHOSEONG SSANGPIEUP: not included in any glyphset definition</li>
<li>U+1109 HANGUL CHOSEONG SIOS: not included in any glyphset definition</li>
<li>U+110A HANGUL CHOSEONG SSANGSIOS: not included in any glyphset definition</li>
<li>U+110B HANGUL CHOSEONG IEUNG: not included in any glyphset definition</li>
<li>U+110C HANGUL CHOSEONG CIEUC: not included in any glyphset definition</li>
<li>U+110D HANGUL CHOSEONG SSANGCIEUC: not included in any glyphset definition</li>
<li>U+110E HANGUL CHOSEONG CHIEUCH: not included in any glyphset definition</li>
<li>U+110F HANGUL CHOSEONG KHIEUKH: not included in any glyphset definition</li>
<li>U+1110 HANGUL CHOSEONG THIEUTH: not included in any glyphset definition</li>
<li>U+1111 HANGUL CHOSEONG PHIEUPH: not included in any glyphset definition</li>
<li>U+1112 HANGUL CHOSEONG HIEUH: not included in any glyphset definition</li>
<li>U+1113 HANGUL CHOSEONG NIEUN-KIYEOK: not included in any glyphset definition</li>
<li>U+1114 HANGUL CHOSEONG SSANGNIEUN: not included in any glyphset definition</li>
<li>U+1115 HANGUL CHOSEONG NIEUN-TIKEUT: not included in any glyphset definition</li>
<li>U+1116 HANGUL CHOSEONG NIEUN-PIEUP: not included in any glyphset definition</li>
<li>U+1117 HANGUL CHOSEONG TIKEUT-KIYEOK: not included in any glyphset definition</li>
<li>U+1118 HANGUL CHOSEONG RIEUL-NIEUN: not included in any glyphset definition</li>
<li>U+1119 HANGUL CHOSEONG SSANGRIEUL: not included in any glyphset definition</li>
<li>U+111A HANGUL CHOSEONG RIEUL-HIEUH: not included in any glyphset definition</li>
<li>U+111B HANGUL CHOSEONG KAPYEOUNRIEUL: not included in any glyphset definition</li>
<li>U+111C HANGUL CHOSEONG MIEUM-PIEUP: not included in any glyphset definition</li>
<li>U+111D HANGUL CHOSEONG KAPYEOUNMIEUM: not included in any glyphset definition</li>
<li>U+111E HANGUL CHOSEONG PIEUP-KIYEOK: not included in any glyphset definition</li>
<li>U+111F HANGUL CHOSEONG PIEUP-NIEUN: not included in any glyphset definition</li>
<li>U+1120 HANGUL CHOSEONG PIEUP-TIKEUT: not included in any glyphset definition</li>
<li>U+1121 HANGUL CHOSEONG PIEUP-SIOS: not included in any glyphset definition</li>
<li>U+1122 HANGUL CHOSEONG PIEUP-SIOS-KIYEOK: not included in any glyphset definition</li>
<li>U+1123 HANGUL CHOSEONG PIEUP-SIOS-TIKEUT: not included in any glyphset definition</li>
<li>U+1124 HANGUL CHOSEONG PIEUP-SIOS-PIEUP: not included in any glyphset definition</li>
<li>U+1125 HANGUL CHOSEONG PIEUP-SSANGSIOS: not included in any glyphset definition</li>
<li>U+1126 HANGUL CHOSEONG PIEUP-SIOS-CIEUC: not included in any glyphset definition</li>
<li>U+1127 HANGUL CHOSEONG PIEUP-CIEUC: not included in any glyphset definition</li>
<li>U+1128 HANGUL CHOSEONG PIEUP-CHIEUCH: not included in any glyphset definition</li>
<li>U+1129 HANGUL CHOSEONG PIEUP-THIEUTH: not included in any glyphset definition</li>
<li>U+112A HANGUL CHOSEONG PIEUP-PHIEUPH: not included in any glyphset definition</li>
<li>U+112B HANGUL CHOSEONG KAPYEOUNPIEUP: not included in any glyphset definition</li>
<li>U+112C HANGUL CHOSEONG KAPYEOUNSSANGPIEUP: not included in any glyphset definition</li>
<li>U+112D HANGUL CHOSEONG SIOS-KIYEOK: not included in any glyphset definition</li>
<li>U+112E HANGUL CHOSEONG SIOS-NIEUN: not included in any glyphset definition</li>
<li>U+112F HANGUL CHOSEONG SIOS-TIKEUT: not included in any glyphset definition</li>
<li>U+1130 HANGUL CHOSEONG SIOS-RIEUL: not included in any glyphset definition</li>
<li>U+1131 HANGUL CHOSEONG SIOS-MIEUM: not included in any glyphset definition</li>
<li>U+1132 HANGUL CHOSEONG SIOS-PIEUP: not included in any glyphset definition</li>
<li>U+1133 HANGUL CHOSEONG SIOS-PIEUP-KIYEOK: not included in any glyphset definition</li>
<li>U+1134 HANGUL CHOSEONG SIOS-SSANGSIOS: not included in any glyphset definition</li>
<li>U+1135 HANGUL CHOSEONG SIOS-IEUNG: not included in any glyphset definition</li>
<li>U+1136 HANGUL CHOSEONG SIOS-CIEUC: not included in any glyphset definition</li>
<li>U+1137 HANGUL CHOSEONG SIOS-CHIEUCH: not included in any glyphset definition</li>
<li>U+1138 HANGUL CHOSEONG SIOS-KHIEUKH: not included in any glyphset definition</li>
<li>U+1139 HANGUL CHOSEONG SIOS-THIEUTH: not included in any glyphset definition</li>
<li>U+113A HANGUL CHOSEONG SIOS-PHIEUPH: not included in any glyphset definition</li>
<li>U+113B HANGUL CHOSEONG SIOS-HIEUH: not included in any glyphset definition</li>
<li>U+113C HANGUL CHOSEONG CHITUEUMSIOS: not included in any glyphset definition</li>
<li>U+113D HANGUL CHOSEONG CHITUEUMSSANGSIOS: not included in any glyphset definition</li>
<li>U+113E HANGUL CHOSEONG CEONGCHIEUMSIOS: not included in any glyphset definition</li>
<li>U+113F HANGUL CHOSEONG CEONGCHIEUMSSANGSIOS: not included in any glyphset definition</li>
<li>U+1140 HANGUL CHOSEONG PANSIOS: not included in any glyphset definition</li>
<li>U+1141 HANGUL CHOSEONG IEUNG-KIYEOK: not included in any glyphset definition</li>
<li>U+1142 HANGUL CHOSEONG IEUNG-TIKEUT: not included in any glyphset definition</li>
<li>U+1143 HANGUL CHOSEONG IEUNG-MIEUM: not included in any glyphset definition</li>
<li>U+1144 HANGUL CHOSEONG IEUNG-PIEUP: not included in any glyphset definition</li>
<li>U+1145 HANGUL CHOSEONG IEUNG-SIOS: not included in any glyphset definition</li>
<li>U+1146 HANGUL CHOSEONG IEUNG-PANSIOS: not included in any glyphset definition</li>
<li>U+1147 HANGUL CHOSEONG SSANGIEUNG: not included in any glyphset definition</li>
<li>U+1148 HANGUL CHOSEONG IEUNG-CIEUC: not included in any glyphset definition</li>
<li>U+1149 HANGUL CHOSEONG IEUNG-CHIEUCH: not included in any glyphset definition</li>
<li>U+114A HANGUL CHOSEONG IEUNG-THIEUTH: not included in any glyphset definition</li>
<li>U+114B HANGUL CHOSEONG IEUNG-PHIEUPH: not included in any glyphset definition</li>
<li>U+114C HANGUL CHOSEONG YESIEUNG: not included in any glyphset definition</li>
<li>U+114D HANGUL CHOSEONG CIEUC-IEUNG: not included in any glyphset definition</li>
<li>U+114E HANGUL CHOSEONG CHITUEUMCIEUC: not included in any glyphset definition</li>
<li>U+114F HANGUL CHOSEONG CHITUEUMSSANGCIEUC: not included in any glyphset definition</li>
<li>U+1150 HANGUL CHOSEONG CEONGCHIEUMCIEUC: not included in any glyphset definition</li>
<li>U+1151 HANGUL CHOSEONG CEONGCHIEUMSSANGCIEUC: not included in any glyphset definition</li>
<li>U+1152 HANGUL CHOSEONG CHIEUCH-KHIEUKH: not included in any glyphset definition</li>
<li>U+1153 HANGUL CHOSEONG CHIEUCH-HIEUH: not included in any glyphset definition</li>
<li>U+1154 HANGUL CHOSEONG CHITUEUMCHIEUCH: not included in any glyphset definition</li>
<li>U+1155 HANGUL CHOSEONG CEONGCHIEUMCHIEUCH: not included in any glyphset definition</li>
<li>U+1156 HANGUL CHOSEONG PHIEUPH-PIEUP: not included in any glyphset definition</li>
<li>U+1157 HANGUL CHOSEONG KAPYEOUNPHIEUPH: not included in any glyphset definition</li>
<li>U+1158 HANGUL CHOSEONG SSANGHIEUH: not included in any glyphset definition</li>
<li>U+1159 HANGUL CHOSEONG YEORINHIEUH: not included in any glyphset definition</li>
<li>U+115A HANGUL CHOSEONG KIYEOK-TIKEUT: not included in any glyphset definition</li>
<li>U+115B HANGUL CHOSEONG NIEUN-SIOS: not included in any glyphset definition</li>
<li>U+115C HANGUL CHOSEONG NIEUN-CIEUC: not included in any glyphset definition</li>
<li>U+115D HANGUL CHOSEONG NIEUN-HIEUH: not included in any glyphset definition</li>
<li>U+115E HANGUL CHOSEONG TIKEUT-RIEUL: not included in any glyphset definition</li>
<li>U+115F HANGUL CHOSEONG FILLER: not included in any glyphset definition</li>
<li>U+1160 HANGUL JUNGSEONG FILLER: not included in any glyphset definition</li>
<li>U+1161 HANGUL JUNGSEONG A: not included in any glyphset definition</li>
<li>U+1162 HANGUL JUNGSEONG AE: not included in any glyphset definition</li>
<li>U+1163 HANGUL JUNGSEONG YA: not included in any glyphset definition</li>
<li>U+1164 HANGUL JUNGSEONG YAE: not included in any glyphset definition</li>
<li>U+1165 HANGUL JUNGSEONG EO: not included in any glyphset definition</li>
<li>U+1166 HANGUL JUNGSEONG E: not included in any glyphset definition</li>
<li>U+1167 HANGUL JUNGSEONG YEO: not included in any glyphset definition</li>
<li>U+1168 HANGUL JUNGSEONG YE: not included in any glyphset definition</li>
<li>U+1169 HANGUL JUNGSEONG O: not included in any glyphset definition</li>
<li>U+116A HANGUL JUNGSEONG WA: not included in any glyphset definition</li>
<li>U+116B HANGUL JUNGSEONG WAE: not included in any glyphset definition</li>
<li>U+116C HANGUL JUNGSEONG OE: not included in any glyphset definition</li>
<li>U+116D HANGUL JUNGSEONG YO: not included in any glyphset definition</li>
<li>U+116E HANGUL JUNGSEONG U: not included in any glyphset definition</li>
<li>U+116F HANGUL JUNGSEONG WEO: not included in any glyphset definition</li>
<li>U+1170 HANGUL JUNGSEONG WE: not included in any glyphset definition</li>
<li>U+1171 HANGUL JUNGSEONG WI: not included in any glyphset definition</li>
<li>U+1172 HANGUL JUNGSEONG YU: not included in any glyphset definition</li>
<li>U+1173 HANGUL JUNGSEONG EU: not included in any glyphset definition</li>
<li>U+1174 HANGUL JUNGSEONG YI: not included in any glyphset definition</li>
<li>U+1175 HANGUL JUNGSEONG I: not included in any glyphset definition</li>
<li>U+1176 HANGUL JUNGSEONG A-O: not included in any glyphset definition</li>
<li>U+1177 HANGUL JUNGSEONG A-U: not included in any glyphset definition</li>
<li>U+1178 HANGUL JUNGSEONG YA-O: not included in any glyphset definition</li>
<li>U+1179 HANGUL JUNGSEONG YA-YO: not included in any glyphset definition</li>
<li>U+117A HANGUL JUNGSEONG EO-O: not included in any glyphset definition</li>
<li>U+117B HANGUL JUNGSEONG EO-U: not included in any glyphset definition</li>
<li>U+117C HANGUL JUNGSEONG EO-EU: not included in any glyphset definition</li>
<li>U+117D HANGUL JUNGSEONG YEO-O: not included in any glyphset definition</li>
<li>U+117E HANGUL JUNGSEONG YEO-U: not included in any glyphset definition</li>
<li>U+117F HANGUL JUNGSEONG O-EO: not included in any glyphset definition</li>
<li>U+1180 HANGUL JUNGSEONG O-E: not included in any glyphset definition</li>
<li>U+1181 HANGUL JUNGSEONG O-YE: not included in any glyphset definition</li>
<li>U+1182 HANGUL JUNGSEONG O-O: not included in any glyphset definition</li>
<li>U+1183 HANGUL JUNGSEONG O-U: not included in any glyphset definition</li>
<li>U+1184 HANGUL JUNGSEONG YO-YA: not included in any glyphset definition</li>
<li>U+1185 HANGUL JUNGSEONG YO-YAE: not included in any glyphset definition</li>
<li>U+1186 HANGUL JUNGSEONG YO-YEO: not included in any glyphset definition</li>
<li>U+1187 HANGUL JUNGSEONG YO-O: not included in any glyphset definition</li>
<li>U+1188 HANGUL JUNGSEONG YO-I: not included in any glyphset definition</li>
<li>U+1189 HANGUL JUNGSEONG U-A: not included in any glyphset definition</li>
<li>U+118A HANGUL JUNGSEONG U-AE: not included in any glyphset definition</li>
<li>U+118B HANGUL JUNGSEONG U-EO-EU: not included in any glyphset definition</li>
<li>U+118C HANGUL JUNGSEONG U-YE: not included in any glyphset definition</li>
<li>U+118D HANGUL JUNGSEONG U-U: not included in any glyphset definition</li>
<li>U+118E HANGUL JUNGSEONG YU-A: not included in any glyphset definition</li>
<li>U+118F HANGUL JUNGSEONG YU-EO: not included in any glyphset definition</li>
<li>U+1190 HANGUL JUNGSEONG YU-E: not included in any glyphset definition</li>
<li>U+1191 HANGUL JUNGSEONG YU-YEO: not included in any glyphset definition</li>
<li>U+1192 HANGUL JUNGSEONG YU-YE: not included in any glyphset definition</li>
<li>U+1193 HANGUL JUNGSEONG YU-U: not included in any glyphset definition</li>
<li>U+1194 HANGUL JUNGSEONG YU-I: not included in any glyphset definition</li>
<li>U+1195 HANGUL JUNGSEONG EU-U: not included in any glyphset definition</li>
<li>U+1196 HANGUL JUNGSEONG EU-EU: not included in any glyphset definition</li>
<li>U+1197 HANGUL JUNGSEONG YI-U: not included in any glyphset definition</li>
<li>U+1198 HANGUL JUNGSEONG I-A: not included in any glyphset definition</li>
<li>U+1199 HANGUL JUNGSEONG I-YA: not included in any glyphset definition</li>
<li>U+119A HANGUL JUNGSEONG I-O: not included in any glyphset definition</li>
<li>U+119B HANGUL JUNGSEONG I-U: not included in any glyphset definition</li>
<li>U+119C HANGUL JUNGSEONG I-EU: not included in any glyphset definition</li>
<li>U+119D HANGUL JUNGSEONG I-ARAEA: not included in any glyphset definition</li>
<li>U+119E HANGUL JUNGSEONG ARAEA: not included in any glyphset definition</li>
<li>U+119F HANGUL JUNGSEONG ARAEA-EO: not included in any glyphset definition</li>
<li>U+11A0 HANGUL JUNGSEONG ARAEA-U: not included in any glyphset definition</li>
<li>U+11A1 HANGUL JUNGSEONG ARAEA-I: not included in any glyphset definition</li>
<li>U+11A2 HANGUL JUNGSEONG SSANGARAEA: not included in any glyphset definition</li>
<li>U+11A3 HANGUL JUNGSEONG A-EU: not included in any glyphset definition</li>
<li>U+11A4 HANGUL JUNGSEONG YA-U: not included in any glyphset definition</li>
<li>U+11A5 HANGUL JUNGSEONG YEO-YA: not included in any glyphset definition</li>
<li>U+11A6 HANGUL JUNGSEONG O-YA: not included in any glyphset definition</li>
<li>U+11A7 HANGUL JUNGSEONG O-YAE: not included in any glyphset definition</li>
<li>U+11A8 HANGUL JONGSEONG KIYEOK: not included in any glyphset definition</li>
<li>U+11A9 HANGUL JONGSEONG SSANGKIYEOK: not included in any glyphset definition</li>
<li>U+11AA HANGUL JONGSEONG KIYEOK-SIOS: not included in any glyphset definition</li>
<li>U+11AB HANGUL JONGSEONG NIEUN: not included in any glyphset definition</li>
<li>U+11AC HANGUL JONGSEONG NIEUN-CIEUC: not included in any glyphset definition</li>
<li>U+11AD HANGUL JONGSEONG NIEUN-HIEUH: not included in any glyphset definition</li>
<li>U+11AE HANGUL JONGSEONG TIKEUT: not included in any glyphset definition</li>
<li>U+11AF HANGUL JONGSEONG RIEUL: not included in any glyphset definition</li>
<li>U+11B0 HANGUL JONGSEONG RIEUL-KIYEOK: not included in any glyphset definition</li>
<li>U+11B1 HANGUL JONGSEONG RIEUL-MIEUM: not included in any glyphset definition</li>
<li>U+11B2 HANGUL JONGSEONG RIEUL-PIEUP: not included in any glyphset definition</li>
<li>U+11B3 HANGUL JONGSEONG RIEUL-SIOS: not included in any glyphset definition</li>
<li>U+11B4 HANGUL JONGSEONG RIEUL-THIEUTH: not included in any glyphset definition</li>
<li>U+11B5 HANGUL JONGSEONG RIEUL-PHIEUPH: not included in any glyphset definition</li>
<li>U+11B6 HANGUL JONGSEONG RIEUL-HIEUH: not included in any glyphset definition</li>
<li>U+11B7 HANGUL JONGSEONG MIEUM: not included in any glyphset definition</li>
<li>U+11B8 HANGUL JONGSEONG PIEUP: not included in any glyphset definition</li>
<li>U+11B9 HANGUL JONGSEONG PIEUP-SIOS: not included in any glyphset definition</li>
<li>U+11BA HANGUL JONGSEONG SIOS: not included in any glyphset definition</li>
<li>U+11BB HANGUL JONGSEONG SSANGSIOS: not included in any glyphset definition</li>
<li>U+11BC HANGUL JONGSEONG IEUNG: not included in any glyphset definition</li>
<li>U+11BD HANGUL JONGSEONG CIEUC: not included in any glyphset definition</li>
<li>U+11BE HANGUL JONGSEONG CHIEUCH: not included in any glyphset definition</li>
<li>U+11BF HANGUL JONGSEONG KHIEUKH: not included in any glyphset definition</li>
<li>U+11C0 HANGUL JONGSEONG THIEUTH: not included in any glyphset definition</li>
<li>U+11C1 HANGUL JONGSEONG PHIEUPH: not included in any glyphset definition</li>
<li>U+11C2 HANGUL JONGSEONG HIEUH: not included in any glyphset definition</li>
<li>U+11C3 HANGUL JONGSEONG KIYEOK-RIEUL: not included in any glyphset definition</li>
<li>U+11C4 HANGUL JONGSEONG KIYEOK-SIOS-KIYEOK: not included in any glyphset definition</li>
<li>U+11C5 HANGUL JONGSEONG NIEUN-KIYEOK: not included in any glyphset definition</li>
<li>U+11C6 HANGUL JONGSEONG NIEUN-TIKEUT: not included in any glyphset definition</li>
<li>U+11C7 HANGUL JONGSEONG NIEUN-SIOS: not included in any glyphset definition</li>
<li>U+11C8 HANGUL JONGSEONG NIEUN-PANSIOS: not included in any glyphset definition</li>
<li>U+11C9 HANGUL JONGSEONG NIEUN-THIEUTH: not included in any glyphset definition</li>
<li>U+11CA HANGUL JONGSEONG TIKEUT-KIYEOK: not included in any glyphset definition</li>
<li>U+11CB HANGUL JONGSEONG TIKEUT-RIEUL: not included in any glyphset definition</li>
<li>U+11CC HANGUL JONGSEONG RIEUL-KIYEOK-SIOS: not included in any glyphset definition</li>
<li>U+11CD HANGUL JONGSEONG RIEUL-NIEUN: not included in any glyphset definition</li>
<li>U+11CE HANGUL JONGSEONG RIEUL-TIKEUT: not included in any glyphset definition</li>
<li>U+11CF HANGUL JONGSEONG RIEUL-TIKEUT-HIEUH: not included in any glyphset definition</li>
<li>U+11D0 HANGUL JONGSEONG SSANGRIEUL: not included in any glyphset definition</li>
<li>U+11D1 HANGUL JONGSEONG RIEUL-MIEUM-KIYEOK: not included in any glyphset definition</li>
<li>U+11D2 HANGUL JONGSEONG RIEUL-MIEUM-SIOS: not included in any glyphset definition</li>
<li>U+11D3 HANGUL JONGSEONG RIEUL-PIEUP-SIOS: not included in any glyphset definition</li>
<li>U+11D4 HANGUL JONGSEONG RIEUL-PIEUP-HIEUH: not included in any glyphset definition</li>
<li>U+11D5 HANGUL JONGSEONG RIEUL-KAPYEOUNPIEUP: not included in any glyphset definition</li>
<li>U+11D6 HANGUL JONGSEONG RIEUL-SSANGSIOS: not included in any glyphset definition</li>
<li>U+11D7 HANGUL JONGSEONG RIEUL-PANSIOS: not included in any glyphset definition</li>
<li>U+11D8 HANGUL JONGSEONG RIEUL-KHIEUKH: not included in any glyphset definition</li>
<li>U+11D9 HANGUL JONGSEONG RIEUL-YEORINHIEUH: not included in any glyphset definition</li>
<li>U+11DA HANGUL JONGSEONG MIEUM-KIYEOK: not included in any glyphset definition</li>
<li>U+11DB HANGUL JONGSEONG MIEUM-RIEUL: not included in any glyphset definition</li>
<li>U+11DC HANGUL JONGSEONG MIEUM-PIEUP: not included in any glyphset definition</li>
<li>U+11DD HANGUL JONGSEONG MIEUM-SIOS: not included in any glyphset definition</li>
<li>U+11DE HANGUL JONGSEONG MIEUM-SSANGSIOS: not included in any glyphset definition</li>
<li>U+11DF HANGUL JONGSEONG MIEUM-PANSIOS: not included in any glyphset definition</li>
<li>U+11E0 HANGUL JONGSEONG MIEUM-CHIEUCH: not included in any glyphset definition</li>
<li>U+11E1 HANGUL JONGSEONG MIEUM-HIEUH: not included in any glyphset definition</li>
<li>U+11E2 HANGUL JONGSEONG KAPYEOUNMIEUM: not included in any glyphset definition</li>
<li>U+11E3 HANGUL JONGSEONG PIEUP-RIEUL: not included in any glyphset definition</li>
<li>U+11E4 HANGUL JONGSEONG PIEUP-PHIEUPH: not included in any glyphset definition</li>
<li>U+11E5 HANGUL JONGSEONG PIEUP-HIEUH: not included in any glyphset definition</li>
<li>U+11E6 HANGUL JONGSEONG KAPYEOUNPIEUP: not included in any glyphset definition</li>
<li>U+11E7 HANGUL JONGSEONG SIOS-KIYEOK: not included in any glyphset definition</li>
<li>U+11E8 HANGUL JONGSEONG SIOS-TIKEUT: not included in any glyphset definition</li>
<li>U+11E9 HANGUL JONGSEONG SIOS-RIEUL: not included in any glyphset definition</li>
<li>U+11EA HANGUL JONGSEONG SIOS-PIEUP: not included in any glyphset definition</li>
<li>U+11EB HANGUL JONGSEONG PANSIOS: not included in any glyphset definition</li>
<li>U+11EC HANGUL JONGSEONG IEUNG-KIYEOK: not included in any glyphset definition</li>
<li>U+11ED HANGUL JONGSEONG IEUNG-SSANGKIYEOK: not included in any glyphset definition</li>
<li>U+11EE HANGUL JONGSEONG SSANGIEUNG: not included in any glyphset definition</li>
<li>U+11EF HANGUL JONGSEONG IEUNG-KHIEUKH: not included in any glyphset definition</li>
<li>U+11F0 HANGUL JONGSEONG YESIEUNG: not included in any glyphset definition</li>
<li>U+11F1 HANGUL JONGSEONG YESIEUNG-SIOS: not included in any glyphset definition</li>
<li>U+11F2 HANGUL JONGSEONG YESIEUNG-PANSIOS: not included in any glyphset definition</li>
<li>U+11F3 HANGUL JONGSEONG PHIEUPH-PIEUP: not included in any glyphset definition</li>
<li>U+11F4 HANGUL JONGSEONG KAPYEOUNPHIEUPH: not included in any glyphset definition</li>
<li>U+11F5 HANGUL JONGSEONG HIEUH-NIEUN: not included in any glyphset definition</li>
<li>U+11F6 HANGUL JONGSEONG HIEUH-RIEUL: not included in any glyphset definition</li>
<li>U+11F7 HANGUL JONGSEONG HIEUH-MIEUM: not included in any glyphset definition</li>
<li>U+11F8 HANGUL JONGSEONG HIEUH-PIEUP: not included in any glyphset definition</li>
<li>U+11F9 HANGUL JONGSEONG YEORINHIEUH: not included in any glyphset definition</li>
<li>U+11FA HANGUL JONGSEONG KIYEOK-NIEUN: not included in any glyphset definition</li>
<li>U+11FB HANGUL JONGSEONG KIYEOK-PIEUP: not included in any glyphset definition</li>
<li>U+11FC HANGUL JONGSEONG KIYEOK-CHIEUCH: not included in any glyphset definition</li>
<li>U+11FD HANGUL JONGSEONG KIYEOK-KHIEUKH: not included in any glyphset definition</li>
<li>U+11FE HANGUL JONGSEONG KIYEOK-HIEUH: not included in any glyphset definition</li>
<li>U+11FF HANGUL JONGSEONG SSANGNIEUN: not included in any glyphset definition</li>
</ul>
<p>Or you can add the above codepoints to one of the subsets supported by the font: <code>latin</code>, <code>latin-ext</code></p>
 [code: unreachable-subsetting]



</div>
</details>

<details>
    <summary>⚠️ <b>WARN</b> Ensure soft_dotted characters lose their dot when combined with marks that replace the dot. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/shaping.html#"></a></summary>
    <div>







* ⚠️ **WARN** <p>The dot of soft dotted characters used in orthographies <em>must</em> disappear in the following strings: i̊ i̋ j̀ j́ j̃ j̄ j̈ į̀ į́ į̂ į̃ į̄ į̌</p>
<p>The dot of soft dotted characters <em>should</em> disappear in other cases, for example: i̇ ǐ ị̇ ị̊ ị̋ ị̌ i̦̇ i̦̊ i̦̋ ǐ̦ i̧̇ i̧̊ i̧̋ ǐ̧ i̱̇ i̱̊ i̱̋ ǐ̱ j̆ j̇</p>
<p>Your font fully covers the following languages that require the soft-dotted feature: Lithuanian (Latn, 2,357,094 speakers), Ebira (Latn, 2,200,000 speakers), Dutch (Latn, 31,709,104 speakers), Igbo (Latn, 27,823,640 speakers), Ekpeye (Latn, 226,000 speakers), Ijo, Southeast (Latn, 2,471,000 speakers).</p>
<p>Your font does <em>not</em> cover the following languages that require the soft-dotted feature: Vute (Latn, 21,000 speakers), Ukrainian (Cyrl, 29,273,587 speakers), Ma’di (Latn, 584,000 speakers), Basaa (Latn, 332,940 speakers), Kpelle, Guinea (Latn, 622,000 speakers), Ejagham (Latn, 120,000 speakers), Fur (Latn, 1,230,163 speakers), Dan (Latn, 1,099,244 speakers), Makaa (Latn, 221,000 speakers), Aghem (Latn, 38,843 speakers), Mundani (Latn, 34,000 speakers), Belarusian (Cyrl, 10,064,517 speakers), Bete-Bendi (Latn, 100,000 speakers), Nzakara (Latn, 50,000 speakers), Southern Kisi (Latn, 360,000 speakers), Dii (Latn, 71,000 speakers), Nateni (Latn, 100,000 speakers), Ngbaka (Latn, 1,020,000 speakers), Mango (Latn, 77,000 speakers), Navajo (Latn, 166,319 speakers), Zapotec (Latn, 490,000 speakers), Sar (Latn, 500,000 speakers), Gulay (Latn, 250,478 speakers), Kom (Latn, 360,685 speakers), Mfumte (Latn, 79,000 speakers), Koonzime (Latn, 40,000 speakers), Bafut (Latn, 158,146 speakers), Avokaya (Latn, 100,000 speakers), Lugbara (Latn, 2,200,000 speakers), Yala (Latn, 200,000 speakers), Cicipu (Latn, 44,000 speakers), South Central Banda (Latn, 244,000 speakers).</p>
 [code: soft-dotted]



</div>
</details>

<details>
    <summary>⚠️ <b>WARN</b> Ensure variable fonts include an avar table. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/googlefonts.varfont.html#"></a></summary>
    <div>







* ⚠️ **WARN** <p>This variable font does not have an avar table.</p>
 [code: missing-avar]



</div>
</details>

<details>
    <summary>⚠️ <b>WARN</b> Ensure fonts have ScriptLangTags declared on the 'meta' table. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/googlefonts.meta.html#"></a></summary>
    <div>







* ⚠️ **WARN** <p>This font file does not have a 'meta' table.</p>
 [code: lacks-meta-table]



</div>
</details>

<details>
    <summary>⚠️ <b>WARN</b> Checking OS/2 achVendID. <a href="https://fontbakery.readthedocs.io/en/stable/fontbakery/checks/googlefonts.os2.html#"></a></summary>
    <div>







* ⚠️ **WARN** <p>OS/2 VendorID value '    ' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at <a href="https://www.microsoft.com/typography/links/vendorlist.aspx">https://www.microsoft.com/typography/links/vendorlist.aspx</a></p>
 [code: unknown]



</div>
</details>
</div>
</details>




### Summary

| 💥 ERROR | ☠ FATAL | 🔥 FAIL | ⚠️ WARN | ⏩ SKIP | ℹ️ INFO | ✅ PASS | 🔎 DEBUG | 
| ---|---|---|---|---|---|---|---|
| 0 | 0 | 8 | 11 | 99 | 8 | 125 | 0 | 
| 0% | 0% | 3% | 4% | 39% | 3% | 50% | 0% | 



**Note:** The following loglevels were omitted in this report:


* SKIP
* INFO
* PASS
* DEBUG
