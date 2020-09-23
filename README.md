<div align="center">

## C\# \- Autocomplete Combo Box


</div>

### Description

C# - Autocomplete Combo Box
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Özgür Aytekin](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/zg-r-aytekin.md)
**Level**          |Intermediate
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |C\#
**Category**       |[GUIs](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/guis__10-30.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/zg-r-aytekin-c-autocomplete-combo-box__10-2165/archive/master.zip)





### Source Code

```
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><B style="mso-bidi-font-weight: normal"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: Verdana; mso-bidi-font-family: 'Courier New'">C# - Autocomplete Combo Box</SPAN></B></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><style="mso-bidi-font-weight: normal"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: Verdana; mso-bidi-font-family: 'Courier New'">www.dotnetcracks.com</SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; COLOR: blue; FONT-FAMILY: 'Courier New'"><?xml:namespace prefix = o ns = "urn:schemas-microsoft-com:office:office" /><o:p> </o:p></SPAN></P><SPAN style="FONT-SIZE: 10pt; COLOR: blue; FONT-FAMILY: 'Courier New'"><SPAN lang=EN-GB style="FONT-SIZE: 10pt; COLOR: blue; FONT-FAMILY: 'Courier New'; mso-ansi-language: EN-GB">
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; COLOR: blue; FONT-FAMILY: 'Courier New'">using</SPAN><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000> System;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; COLOR: blue; FONT-FAMILY: 'Courier New'">using</SPAN><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000> System.Windows.Forms;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><o:p><FONT color=#000000> </FONT></o:p></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; COLOR: blue; FONT-FAMILY: 'Courier New'">namespace</SPAN><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000> Dotnetcracks<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000>{<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 1"><FONT color=#000000>      </FONT></SPAN><SPAN style="COLOR: blue">public</SPAN><FONT color=#000000> </FONT><SPAN style="COLOR: blue">class</SPAN><FONT color=#000000> AutoCompleteComboBox : ComboBox<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 1">      </SPAN>{<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 2"><FONT color=#000000>            </FONT></SPAN><SPAN style="COLOR: green">// Autocomple Combo Box<o:p></o:p></SPAN></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 2"><FONT color=#000000>            </FONT></SPAN><SPAN style="COLOR: blue">private</SPAN><FONT color=#000000> </FONT><SPAN style="COLOR: blue">bool</SPAN><FONT color=#000000> _controlKey = </FONT><SPAN style="COLOR: blue">false</SPAN><FONT color=#000000>;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><o:p><FONT color=#000000> </FONT></o:p></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 2"><FONT color=#000000>            </FONT></SPAN><SPAN style="COLOR: blue">protected</SPAN><FONT color=#000000> </FONT><SPAN style="COLOR: blue">override</SPAN><FONT color=#000000> </FONT><SPAN style="COLOR: blue">void</SPAN><FONT color=#000000> OnKeyPress(KeyPressEventArgs e)<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 2">            </SPAN>{<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 3"><FONT color=#000000>                  </FONT></SPAN><SPAN style="COLOR: blue">base</SPAN><FONT color=#000000>.OnKeyPress (e);<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><o:p><FONT color=#000000> </FONT></o:p></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 3"><FONT color=#000000>                  </FONT></SPAN><SPAN style="COLOR: blue">if</SPAN><FONT color=#000000> (e.KeyChar == (</FONT><SPAN style="COLOR: blue">int</SPAN><FONT color=#000000>)Keys.Escape)<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 3">                  </SPAN>{<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 4"><FONT color=#000000>                        </FONT></SPAN><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>.SelectedIndex = -1;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 4"><FONT color=#000000>                        </FONT></SPAN><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>.Text = String.Empty;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 4">                        </SPAN><o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 4"><FONT color=#000000>                        </FONT></SPAN><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>._controlKey = </FONT><SPAN style="COLOR: blue">true</SPAN><FONT color=#000000>;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 3">                  </SPAN>}<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 3"><FONT color=#000000>                  </FONT></SPAN><SPAN style="COLOR: blue">else</SPAN><FONT color=#000000> </FONT><SPAN style="COLOR: blue">if</SPAN><FONT color=#000000> (Char.IsControl(e.KeyChar))<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 3">                  </SPAN>{<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 4"><FONT color=#000000>                        </FONT></SPAN><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>._controlKey = </FONT><SPAN style="COLOR: blue">true</SPAN><FONT color=#000000>;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 3">                  </SPAN>}<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 3"><FONT color=#000000>                  </FONT></SPAN><SPAN style="COLOR: blue">else<o:p></o:p></SPAN></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 3">                  </SPAN>{<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 4"><FONT color=#000000>                        </FONT></SPAN><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>._controlKey = </FONT><SPAN style="COLOR: blue">false</SPAN><FONT color=#000000>;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 3">                  </SPAN>}<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 2">            </SPAN>}<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><o:p><FONT color=#000000> </FONT></o:p></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 2"><FONT color=#000000>            </FONT></SPAN><SPAN style="COLOR: blue">protected</SPAN><FONT color=#000000> </FONT><SPAN style="COLOR: blue">override</SPAN><FONT color=#000000> </FONT><SPAN style="COLOR: blue">void</SPAN><FONT color=#000000> OnTextChanged(EventArgs e)<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 2">            </SPAN>{<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 3"><FONT color=#000000>                  </FONT></SPAN><SPAN style="COLOR: blue">base</SPAN><FONT color=#000000>.OnTextChanged (e);<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><o:p><FONT color=#000000> </FONT></o:p></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 3"><FONT color=#000000>                  </FONT></SPAN><SPAN style="COLOR: blue">if</SPAN><FONT color=#000000> (</FONT><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>.Text != String.Empty && !</FONT><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>._controlKey)<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 3">                  </SPAN>{<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 4"><FONT color=#000000>                        </FONT></SPAN><SPAN style="COLOR: blue">string</SPAN><FONT color=#000000> strMatchText = </FONT><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>.Text;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 4"><FONT color=#000000>                        </FONT></SPAN><SPAN style="COLOR: blue">int</SPAN><FONT color=#000000> intMatchPos = </FONT><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>.FindString(strMatchText);<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><o:p><FONT color=#000000> </FONT></o:p></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 4"><FONT color=#000000>                        </FONT></SPAN><SPAN style="COLOR: blue">if</SPAN><FONT color=#000000> (intMatchPos != -1)<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 4">                        </SPAN>{<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 5"><FONT color=#000000>                              </FONT></SPAN><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>.SelectedIndex = intMatchPos;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><o:p><FONT color=#000000> </FONT></o:p></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 5"><FONT color=#000000>                              </FONT></SPAN><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>.SelectionStart = strMatchText.Length;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><SPAN style="mso-tab-count: 5"><FONT color=#000000>                              </FONT></SPAN><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>.SelectionLength = </FONT><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>.Text.Length - </FONT><SPAN style="COLOR: blue">this</SPAN><FONT color=#000000>.SelectionStart;<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 4">                        </SPAN>}<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 3">                  </SPAN>}<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 2">            </SPAN>}<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000><SPAN style="mso-tab-count: 1">      </SPAN>}<o:p></o:p></FONT></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><FONT color=#000000>}</FONT></SPAN></SPAN></SPAN><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: 'Courier New'"><o:p> </o:p></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; mso-layout-grid-align: none"><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: Verdana; mso-bidi-font-family: 'Courier New'"><o:p> </o:p></SPAN></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; TEXT-ALIGN: right" align=right><?xml:namespace prefix = st1 ns = "urn:schemas-microsoft-com:office:smarttags" /><st1:personname w:st="on"><SPAN style="FONT-SIZE: 10pt; COLOR: black; FONT-FAMILY: Verdana">Özgür Aytekin (MCSD .NET, MCDBA)</SPAN></st1:personname></P>
<P class=MsoNormal style="MARGIN: 0in 0in 0pt; TEXT-ALIGN: right" align=right><SPAN style="FONT-SIZE: 10pt; COLOR: black; FONT-FAMILY: Verdana"></SPAN><SPAN style="FONT-SIZE: 10pt; FONT-FAMILY: Verdana"><o:p></o:p></SPAN></P>
```

