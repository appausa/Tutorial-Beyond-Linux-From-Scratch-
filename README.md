# Tutorial-Beyond-Linux-From-Scratch-
Muestro el orden de Intalacion de BLFS y los pasos a seguir

# Estos primeros son necesarios para la instalación

**Nota: No importan las dependencias en estos.**
1. Wget-1.25.0 (Necesario para las descargas)
2. Nano-8.7.1 (Es mi editador preferido)
3. OpenSSH-10.2p1 (Para intalar de forma remota)
4. blfs-systemd-units-20251204 (Necesario durante toda la instalación)
5. GPM-1.20.7 (Para usar el mouse por consola)

**El momento de la verdad**
1. libevent-2.1.12
2. links-2.30
3. NSPR-4.38.2
4. libgpg-error-1.59
5. LZO-2.10
6. icu-78.2
7. Nettle-3.10.2
8. libxml2-2.15.1
9. npth-1.8
10. libarchive-3.8.5
11. SQLite-3.50.4 (No viene en la versión 13)
12. sgml-common-0.6.3
13. libtasn1-4.21.0
14. libtirpc-1.3.6
15. libnsl-2.0.1
16. libgcrypt-1.12.0
17. docbook-xsl-nons-1.79.2
18. docbook-xml-4.5
19. libxslt-1.1.45
20. Zip-3.0
21. Sharutils-4.15.2
22. rpcsvc-proto-1.4.4
23. NSS-3.120.1
24. docbook-xml-5.0
25. p11-kit-0.26.2
26. make-ca-1.16.1
27. Berkeley db-5.3.28 (No viene en la version 13)
28. CrackLib-2.10.3
29. libpwquality-1.4.5
30. lynx2.9.2
31. Linux-PAM-1.7.2
32. libpwquality-1.4.5 (Segunda Vez)
33. Linux-PAM-1.7.2 (Segunda Vez)
34. Shadow-4.19.3
35. Sudo-1.9.17p2
36. libunistring-1.4.1
37. lmdb-0.9.35
38. Cyrus SASL-2.1.28
39. unixODBC-2.3.14
40. OpenLDAP-2.6.12
41. sendmail.8.18.1 (No viene en la version 13)
42. Archive::Zip-1.68 (Perl)
43. autovivification-0.18 (Perl)
44. Business::ISBN::Data-20260214.001 (Perl)
45. Business::ISBN-3.012 (Perl)
46. Tie::Cycle-1.233 (Perl)
47. Business::ISMN-1.205 (Perl)
48. Business::ISSN-1.008 (Perl)
49. Class::Accessor-0.51 (Perl)
50. B::COW-0.007 (Perl)
51. Number::Compare-0.03 (Perl)
52. Text::Glob-0.11 (Perl)
53. File::Find::Rule-0.35 (Perl)
54. Data::Compare-1.29 (Perl)
55. Data::Dump-1.25 (Perl)
56. Data::Uniqid-0.12 (Perl)
57. Encode::HanExtra-0.23 (Perl)
58. Encode::JIS2K-0.05 (Perl)
59. File::FcntlLock-0.22 (Perl)
60. Test::Warnings-0.038 (Perl)
61. File::Slurper-0.014 (Perl)
62. Test::Warnings-0.038 (Perl)
63. File::Which-1.27 (Perl)
64. HTML::Tagset-3.24 (Perl)
65. Encode::Locale-1.05 (Perl)
66. TimeDate-2.33 (Perl)
67. HTTP::Date-6.06 (Perl)
68. IO::HTML-1.004 (Perl)
60. Capture::Tiny-0.50 (Perl)
70. Try::Tiny-0.32 (Perl)
71. Test::Fatal-0.018 (Perl)
72. LWP::MediaTypes-6.04 (Perl)
73. MIME::Base32-1.303 (Perl)
74. Test::Needs-0.002010 (Perl)
75. URI-5.34 (Perl)
76. HTTP::Message-7.01 (Perl)
77. HTML::Parser-3.83 (Perl)
78. HTTP::Daemon-6.16 (Perl)
79. Net::SSLeay-1.94 (Perl)
80. IO::String-1.08 (Perl)
81. IPC::Run3-0.049 (Perl)
82. File::Listing-6.16 (Perl)
83. Lingua::Translit-0.29 (Perl)
84. Test::Deep-1.205 (Perl)
85. Test::Requires-0.11 (Perl)
86. HTTP::CookieJar-0.014 (Perl)
87. HTTP::Cookies-6.11 (Perl)
88. HTTP::Negotiate-6.01 (Perl)
89. Test::RequiresInternet-0.05 (Perl)
90. LWP (libwww-perl-6.81) (Perl)
91. WWW::RobotRules-6.02 (Perl)
92. LWP (libwww-perl-6.81) (Perl) (Segunda vez)
93. Module::Runtime-0.018 (Perl)
94. Test::LeakTrace-0.17 (Perl)
95. List::UtilsBy-0.12 (Perl)
96. Module::Implementation-0.09 (Perl)
97. List::SomeUtils::XS-0.58 (Perl)
98. List::SomeUtils-0.59 (Perl)
99. List::AllUtils-0.19 (Perl)
100. Exporter::Tiny-1.006003 (Perl)
101. List::MoreUtils::XS-0.430 (Perl)
102. List::MoreUtils-0.430 (Perl)
103. Log::Log4perl-1.57 (Perl)
104. Module::Build-0.4234 (Perl)
105. Net::DNS-1.54 (Perl)
106. Parse::RecDescent-1.967015 (Perl)
107. Parse::Yapp-1.21 (Perl)
108. Sub::Uplevel-0.2800 (Perl)
109. Test::Exception-0.43 (Perl)
110. PerlIO::utf8_strict-0.010 (Perl)
111. Regexp::Common-2024080801 (Perl)
112. SGMLSpm-1.1 (Perl)
113. Encode::EUCJPASCII-0.03 (Perl)
114. IO::Socket::SSL-2.098 (Perl)
115. LWP::Protocol::https-6.14 (Perl)
116. Sort::Key-1.33 (Perl)
117. docbook-3.1-dtd
118. docbook-4.5-dtd
119. xmlto-0.0.29
120. OpenSP-1.5.2
121. OpenJade-1.3.2
122. docbook-dsssl-1.79
123. DocBook-utils-0.6.14
124. Which-2.23 and Alternatives
125. Fcron-3.4.0
126. util-macros-1.20.2
127. GLM-1.0.3
128. xbitmaps-1.1.3
129. Asciidoc-10.2.1 (Python)
130. xorgproto-2025.1
131. libXau-1.0.12
132. libXdmcp-1.1.5
133. xcb-proto-1.17.0
134. libxcb-1.17.0
135. libseccomp-2.6.0
136. Bubblewrap-0.11.0
137. Fontconfig-2.17.1
138. Xorg Libraries
139. Introduction to Xorg-7
140. libxcvt-0.1.3
141. xcb-util-0.4.1
142. XCB Utilities
143. libpng-1.6.55
144. slang-2.3.3
145. libaio-0.3.113
146. dbus-1.16.2 1ra Vez
147. CMake-4.2.3
148. libidn2-2.3.8
149. libpsl-0.21.5
150. libssh2-1.11.1
151. libyaml-0.2.5
152. libassuan-3.0.2
153. libksba-1.6.7
154. libuv-1.52.0
155. Patchelf-0.18.0
156. brotli-1.2.0
157. Editables-0.5 (Python)
158. Pathspec-1.0.4 (Python)
159. Pyproject_Hooks-1.2.0 (Python)
160. build-1.4.0 (Python)
161. docutils-0.22.4 (Python)
162. Alabaster-1.0.0 (Python)
163. Pytz-2025.2 (Python)
164. babel-2.18.0 (Python)
165. Cython-3.2.4 (Python)
166. Pyproject-Metadata-0.11.0 (Python)
167. Meson_python-0.19.0 (Python)
168. NumPy-2.4.2 (Python)
169. Py3c-1.4 (Python)
170. c-ares-1.34.6
171. Apr-1.7.6
172. boost-1.90.0
173. Ruby-4.0.1
174. MariaDB-11.8.6
175. Apr-Util-1.6.3
176. Jansson-2.15.0
177. Lua-5.4.8
178. Popt-1.19
179. rsync-3.4.1
180. Apache-2.4.66
181. stunnel-5.77
182. cURL-8.18.0
