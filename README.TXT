Glósur fyrir css/js vegna Sálmaskýringaverkefnis

Header með linkum sem skipta milli Sálmaskýringa, Biblíutexta og Tónlistarskýringa auk hugsanlega fleiri möguleika eins og upplýsingum um höfund texta, höfund lags, mikið notaðar/dæmigerðar útsetningar og fleira í þeim dúr.
Transistion milli síðna renni eins og sé dregið til hliðar á snertiskjá, þegar skoðað er á raunverulegum snertiskjá sé hægt að draga á þennan hátt á milli.
Header skipti í réttan lit eftir sálmum miðað við kirkjuár.
Allir takkar séu rúnnaðir með box-shadow border en fully transparent svo bakgrunnur sjáist í gegn.
Bakgrunnur sé einskonar mjög ljóst olíumix með svartan texta (og borders) eða mjög dökkt olíumix með hvítan texta (og borders), alveg augljóst hvar og hvernig eigi að skipta á milli. Í bili, fyrir demo, má nota circular gradient til að fá fram næstum því réttu áhrifunum. Annar möguleiki eru opnar myndir frá NASA af hinum og þessum geimskýjum.
Sidebar sýni texta sálms á sálmaskýringasíðu og biblíutextasíðu, nótur að lagi (þar sem fæst leyfi, annars líka texta sálms) á tónlistarskýringasíðu. Á síðu um höfund lags eða höfund texta sé mynd af viðkomandi ef hún er til, á síðu um útsetningar séu myndir af þeim sem útsettu.

Fyrir hvern sálm þarf að halda utan um id (serial, primary key), höfund (varchar(#)), þýðanda ef við á (varchar(#)), ártal saminn (int), ártal þýddur (int), lagahöfund (varchar(#)), ártal lags (int), textann í heild (text), skýringarnar (text, titillinn fremstur aðskilinn frá með ';'), nótnamynd (lob), biblíutexta (text, vísun fremst aðskilin frá með ';'), númer í nýjustu sálmabók ef hann er þar (int), frumtexta ef þýddur (text, titillinn fremstur aðskilinn frá með ';'), hvaðan þýddur ef við á (varchar(#)), elstu þekktu heimild ef við á (varchar(#)).