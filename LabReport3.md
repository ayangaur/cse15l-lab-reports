# CSE 15L Lab Report 3 Ayan Gaur

## `grep` Command

The `grep` command has many ways to use it. 
https://phoenixnap.com/kb/grep-command-linux-unix-examples shows various ways to use the grep command. Using this website I have picked the following extensions.

In the examples below, I will only be showing some of the results since all the results would be very long and would take up too much space.

### 1. To find whole words
`grep -w` can be used to find whole words instead of just the specific pattern in the text file.

```
Ayans-MacBook-Pro:written_2 ayan$ grep -w "India" */*/*
grep: non-fiction/OUP/Abernathy: Is a directory
grep: non-fiction/OUP/Berk: Is a directory
grep: non-fiction/OUP/Castro: Is a directory
grep: non-fiction/OUP/Fletcher: Is a directory
grep: non-fiction/OUP/Kauffman: Is a directory
grep: non-fiction/OUP/Rybczynski: Is a directory
travel_guides/berlitz1/HistoryEgypt.txt:        dominions in India, the Far East, Australia, and New Zealand. When the
travel_guides/berlitz1/HistoryFWI.txt:        of some 80,000 Hindus from India and 16,000 free Africans began
travel_guides/berlitz1/HistoryFrance.txt:        Indochinese peace settlement. He handed Pondicherry over to India and
travel_guides/berlitz1/HistoryGreek.txt:        as India, the Aegean became a crossroads for the long trading routes.
travel_guides/berlitz1/HistoryHongKong.txt:        connections in India and the Middle East. By a.d. 900, the Hong Kong
travel_guides/berlitz1/HistoryHongKong.txt:        solve the problem. Grown in India, it was delivered to Canton, and
travel_guides/berlitz1/HistoryIndia.txt:        India has always been a melange of peoples. Apart from some
travel_guides/berlitz1/HistoryIndia.txt:        pre-Ice Age hominids, the first settlers to arrive in India were
travel_guides/berlitz1/HistoryIndia.txt:        then on to Iran before entering India. These fair-skinned
travel_guides/berlitz1/HistoryIndia.txt:        took to the asceticism which has characterized spiritual life in India.
travel_guides/berlitz1/HistoryIndia.txt:        invaders appeared at India’s frontiers; Cyrus, Emperor of Persia,
travel_guides/berlitz1/HistoryIndia.txt:        lasting impact on India during the two-year campaign.
travel_guides/berlitz1/HistoryIndia.txt:        Maurya (321–297 b.c. ), was also to become the founder of India’s first
travel_guides/berlitz1/HistoryIndia.txt:        elephants, chariots, and infantry. Southern India remained independent,
travel_guides/berlitz1/HistoryIndia.txt:        the northern half of India and into Central Asia. His reign was one of
travel_guides/berlitz1/HistoryIndia.txt:        prosperity, making India a trade center between east and west.
travel_guides/berlitz1/HistoryIndia.txt:        arts also flourished in India during these early times. Madurai was the
travel_guides/berlitz1/HistoryIndia.txt:        many bounties, such as silk, musk, and amber, in exchange for India’s
travel_guides/berlitz1/HistoryIndia.txt:        reigned for 40 years over northern India, and encouraged Buddhist monks
travel_guides/berlitz1/HistoryIndia.txt:        In southern India, power was shared by the Pallavas in
travel_guides/berlitz1/HistoryIndia.txt:        Islam Comes to India
```
Only results from where the word India is used are shown and words like 'Indian' which contain 'India' in them do not show up.

```
Ayans-MacBook-Pro:written_2 ayan$ grep -w "group" */*/*
grep: non-fiction/OUP/Abernathy: Is a directory
grep: non-fiction/OUP/Berk: Is a directory
grep: non-fiction/OUP/Castro: Is a directory
grep: non-fiction/OUP/Fletcher: Is a directory
grep: non-fiction/OUP/Kauffman: Is a directory
grep: non-fiction/OUP/Rybczynski: Is a directory
travel_guides/berlitz1/HistoryEdinburgh.txt:        fierce group called the Picts, whom they drove north. They consolidated
travel_guides/berlitz1/HistoryEdinburgh.txt:        Votadini. Little is recorded about this group, but they were probably
travel_guides/berlitz1/HistoryEdinburgh.txt:        The next year, a large group of Scottish churchmen and
travel_guides/berlitz1/HistoryEgypt.txt:        In June 1952 a group of high-ranking military officers
travel_guides/berlitz1/HistoryIndia.txt:        group of liberal Hindu and Parsi intellectuals, supported by a few
travel_guides/berlitz1/HistoryIndia.txt:        Center group as government within the British Empire, and by a
travel_guides/berlitz1/HistoryIndia.txt:        breakaway revolutionary Extreme Left group as complete
travel_guides/berlitz1/HistoryIndia.txt:        a separate Muslim homeland in the northwest of India. A small group of
travel_guides/berlitz1/HistoryIsrael.txt:        many lands. So Abraham, the first Patriarch, led his nomadic group of
travel_guides/berlitz1/HistoryIstanbul.txt:        democracy. These intellectuals form­ed an underground group known as
travel_guides/berlitz1/HistoryJapan.txt:        prestigious group was ensured by cementing their ethical principles in
travel_guides/berlitz1/HistoryJapan.txt:        debate and confrontation and the group-oriented preference for
travel_guides/berlitz1/HistoryLakeDistrict.txt:        wreaking havoc, however, a small but influential group of writers and
travel_guides/berlitz1/HistoryLakeDistrict.txt:        and its lifestyle. William Wordsworth, the most famous of the group,
travel_guides/berlitz1/HistoryLakeDistrict.txt:        natural valley, a group of concerned individuals formed the Lake
travel_guides/berlitz1/IntroGreek.txt:        of the Turkish coastline. The major island in the group is Rhodes
travel_guides/berlitz1/IntroIndia.txt:        group in India — almost as many as the population of Pakistan — most of
travel_guides/berlitz1/IntroJamaica.txt:        come across a friendly conversation among a group of friends. The loud,
travel_guides/berlitz1/IntroJapan.txt:        A third group, not of different ethnic origin from the
travel_guides/berlitz1/IntroJerusalem.txt:        group that broke away from Islam in the 11th century and now live
travel_guides/berlitz1/IntroLakeDistrict.txt:        railway line through the heart of the region — galvanized a small group
travel_guides/berlitz1/IntroLakeDistrict.txt:        Revolution, a group of 19th-century writers, known collectively as the
travel_guides/berlitz1/IntroLasVegas.txt:        to serve an already-waiting group of customers. Driving through these
travel_guides/berlitz1/IntroLosAngeles.txt:        comprise the largest ethnic group of all, with numbers fast approaching
travel_guides/berlitz1/IntroMadeira.txt:        tip of a submerged mass. Only one other island in the small group is
travel_guides/berlitz1/WhatToFWI.txt:        join an organized group excursion following country trails through
travel_guides/berlitz1/WhatToFWI.txt:        Ballets Martiniquais Folklore group perform traditional local
travel_guides/berlitz1/WhatToIbiza.txt:        group. They are renowned as far away as New York for their Ibiza look.
travel_guides/berlitz1/WhatToJamaica.txt:        the eastern group (the western Maroon area is in Cockpit Country, south
travel_guides/berlitz1/WhatToLakeDistrict.txt:        For information about lessons and/or guided group excursions
travel_guides/berlitz1/WhatToLakeDistrict.txt:        For information about lessons and/or group excursions, try
travel_guides/berlitz1/WhatToLasVegas.txt:        extraordinary illusions with the assistance of a talented group of
travel_guides/berlitz1/WhereToDublin.txt:        entrance fee, adults IR£1.20, children 50p; go early to avoid group
travel_guides/berlitz1/WhereToEdinburgh.txt:        take pride of place — the zoo has the world’s largest group in
travel_guides/berlitz1/WhereToEgypt.txt:        new group of deities.
travel_guides/berlitz1/WhereToEgypt.txt:        Habu. Often left out of the tour group itinerary, this part of the west
```

### 2. To search all subdirectories
`grep -r` can be used to search through all the subdirectories of a directory instead of having to check them individually.

```
Ayans-MacBook-Pro:written_2 ayan$ grep -r "farther" *
non-fiction/OUP/Rybczynski/ch3.txt:Early in his career, after emigrating to the United States from South Africa, Greenberg was employed writing design standards for courthouses, which led to an unusual commission: the conversion of an empty supermarket into a courthouse. He gave the commercial building in Manchester, Connecticut, a new façade dominated by a large arch, over-scaled voussoirs, and a pediment. Inside, the barrel-vaulted ceiling of the lobby was supported by a Tuscan order. Greenberg had graduated from Yale in 1965, and like many of his contemporaries was experimenting with the new freedom offered by Postmodernism. However, unlike Venturi and Moore, Greenberg was not coyly introducing Classical elements into a Modernist building; he was returning to Classical roots. From this modest beginning, over the next two decades, came a variety of commissions: a suite of rooms for the Secretary of State in the United States Department of State building, several college and university buildings, and a Roman Catholic church. His commercial work included a newspaper office building in Athens, Georgia, a new entrance for Bergdorf Goodman on Fifth Avenue in Manhattan, and a flagship store for Tommy Hilfiger in Beverly Hills. Greenberg is also known for large country houses, both in the United States and in Europe. Like Lutyens and John Russell Pope, he ventures stylistically farther afield in his residential work—using Georgian and American Colonial styles. One of his early houses was inspired by Mount Vernon, another by Palladio’s unfinished Villa Thiene. Several are picturesque rambling affairs whose relaxed informality recalls the best work of McKim, Mead & White.
travel_guides/berlitz1/HistoryItaly.txt:        trade with Muslims and others farther east. The merchants of Venice
travel_guides/berlitz1/WhereToGreek.txt:        Most commercial ferries arrive at the new port of Athinios farther
travel_guides/berlitz1/WhereToGreek.txt:        that of their neighbors farther south in the Aegean.
travel_guides/berlitz1/WhereToLakeDistrict.txt:        District, if not the most dramatic visually. (You’ll have to go farther
travel_guides/berlitz1/WhereToLakeDistrict.txt:        a good base for trips farther afield in the Lakes.
travel_guides/berlitz1/WhereToLakeDistrict.txt:        leads farther along the eastern shore of the lake to Martindale with
travel_guides/berlitz1/WhereToLakeDistrict.txt:        (2 miles) farther down the road is the Sharrow Bay Hotel, the first and
travel_guides/berlitz1/WhereToLakeDistrict.txt:        A few kilometers farther south you’ll come upon “Surprise
travel_guides/berlitz1/WhereToLakeDistrict.txt:        Just a little farther along the valley to the northwest,
travel_guides/berlitz1/IntroMadrid.txt:        two decades, has pushed farther and farther out, leaving little
travel_guides/berlitz1/HistoryIstanbul.txt:        farther still into India. During his 12-year campaign Alexander
travel_guides/berlitz1/WhereToItaly.txt:        farther afield — west to Pisa and Lucca before turning south through
travel_guides/berlitz1/WhereToItaly.txt:        farther out in the lake, is the largest and most peaceful of the
travel_guides/berlitz1/WhereToItaly.txt:        Herculaneum, the Vesuvius volcano, and farther down the coast, the
travel_guides/berlitz1/WhereToMalaysia.txt:        kilometers (7 miles) farther brings you to Tanah Rata, the main
travel_guides/berlitz1/WhereToMalaysia.txt:        British cemetery is to be found farther down the hill.
travel_guides/berlitz1/WhereToMalaysia.txt:        farther north. Pantai Seri Tujuh (“Beach of the Seven Lagoons”), about
travel_guides/berlitz1/WhereToMalaysia.txt:        Merang (not to be confused with the town of Marang farther south).
travel_guides/berlitz1/WhereToMalaysia.txt:        farther north. Facilities around the main island port of Tekek include
travel_guides/berlitz1/WhereToMalaysia.txt:        town center. Desaru is 52 km (32 miles) farther east and is the first
travel_guides/berlitz1/WhereToMalaysia.txt:        its lively nightlife, to shop, or to head farther north. Outside the
travel_guides/berlitz1/WhereToMalaysia.txt:        in the 1850s, is here. Still farther west, the Kuching Mosque, built in
travel_guides/berlitz1/WhereToMalaysia.txt:        alternative being to travel even farther into the forests at added
travel_guides/berlitz1/WhereToMalaysia.txt:        from KK, and farther north at Kota Belud, where one finds the
travel_guides/berlitz1/WhatToMalaysia.txt:        beach of Rantau Abang, and farther south at Johor’s Desaru, haven’t yet
travel_guides/berlitz1/WhereToJapan.txt:        Still farther south is the Tsukiji Central Wholesale
travel_guides/berlitz1/WhereToJapan.txt:        Still farther south is Kenchoji, founded in 1249, the foremost of the
travel_guides/berlitz1/WhereToEdinburgh.txt:        Observatory was relocated to Blackford Hill, farther south, in 1895.
travel_guides/berlitz1/WhereToIsrael.txt:        little farther along until you come to the landmark Rockefeller Museum,
travel_guides/berlitz1/WhereToIsrael.txt:        farther out to sea without getting your feet wet, Coral World also has
travel_guides/berlitz1/WhereToFrance.txt:        with her first birth pains. She made it no farther than a first-floor
travel_guides/berlitz1/WhereToFrance.txt:        40,000 years old. The Combarelles cave, farther to the east, is a long
travel_guides/berlitz1/IntroIstanbul.txt:        farther.
travel_guides/berlitz1/WhereToMallorca.txt:        farther on.
```

Using the `-r` extension, we went through all the subdirectories of `written_2` We can see the results from `non-fiction` and `travel_guides`. The actual results show the results from `berlitz2` as well.

```
Ayans-MacBook-Pro:written_2 ayan$ grep -r "Bahamas" *
travel_guides/berlitz1/WhatToFWI.txt:        waters off the Bahamas, Puerto Rico, and the Virgin Islands, but the
travel_guides/berlitz2/Bahamas-WhereToGo.txt:It’s not the largest of the Bahamas islands and not the most stunningly beautiful, yet when most people think of the Bahamas they first think of New Providence or its major town, Nassau. The island is only 80 square miles in size yet 180,000 of the 280,000 Bahamians lives here. The town and its port and international airport are the hub for every activity in the Bahamas. Government, administration, taxes, and furniture shipments for new homes all start from here and radiate out to the other islands. New Providence also attracts over 3 million visitors every year, and Nassau is one of the main cruise ports of the Caribbean. The island is a magnet for fun seekers and serious shoppers, and it serves both very well.
travel_guides/berlitz2/Bahamas-WhereToGo.txt:Nassau town has a fine pedigree dating back through colonial times, and the compact town center still has the feel of life under the English. Out in the natural harbor, which offered shelter to many a pirate ship, is a major port that can accommodate 15 large cruise ships at one time. This capacity was created in 1965 when public money was invested to dredge the port, specifically to allow bigger ships to enter. The huge vessels, hundreds of feet high, dwarf the towns buildings, which regulations set at a maximum of three stories, and create one of the most effective juxtapositions of modernity and history found anywhere in the world. The cruise port at Prince George Wharf brings in by far the majority of visitors to the Bahamas.
travel_guides/berlitz2/Bahamas-WhereToGo.txt:The first sight that will attract your attention is the Straw Market on Market Plaza, which backs onto Woodes Rodgers Walk. For many years this has been the showcase for Bahamian handicrafts. Straw goods, including baskets and mats, are favorite souvenirs; each island produces straw goods in its own style and patterns. Bestsellers are hats, dolls, bags, and baskets. There is some exquisite work to be found, but be aware that with a decline in basket-making throughout the Bahamas, an increasing number of articles are imported from the Far East; most of these are at the cheaper end of the scale. The ubiquitous modern souvenir, the T-shirt, is also available, with an almost limitless number of pictures, patterns, and slogans. The ladies who run the stalls are easy-going and seem to have limitless enthusiasm for the next sale. You’ll hear numerous calls of “Hey, honey, come look for something nice here.”
travel_guides/berlitz2/Bahamas-WhereToGo.txt:The straw market fronts onto Bay Street, one of the leading duty-free shopping capitals of the world. Only a few years ago this street was the domain of the Bay Street Boys, a small group of men who controlled all economic activity in the Bahamas; now Bay Street seduces visitors with huge sparkling gems, hundreds of ounces of gold, and the smell of a thousand designer fragrances. The façades of the pretty 18th-century shops hide modern air-conditioned shopping palaces piled high with luxury goods.
travel_guides/berlitz2/Bahamas-WhereToGo.txt:Behind the modern law court complex is the Nassau Public Library, interesting because it used to be the island’s jail. The octagonal structure on Shirley Street dates from 1797 and has a pretty exterior, but the interior is more fascinating. The old cells were retained when the structure became the library in 1873 and books line every wall, replacing prisoners and creating private reading areas. The library museum also has a collection of old maps and charts used to navigate the waters around the Bahamas.
travel_guides/berlitz2/Bahamas-WhereToGo.txt:The resort boasts 20 restaurants, three shopping malls, and a vast casino area. Outside, water slides, nature trails, and swimming pools indicate that no expense has been spared to create the ultimate playground for all age groups. Many visitors to the Bahamas drop in just to marvel at the artistry and technical skill that was employed to create this complex. Non-guests must pay a fee to enjoy the resort facilities and an extra fee for a visit to the Dig.
travel_guides/berlitz2/Bahamas-WhereToGo.txt:Head west out of Nassau and within a couple of minutes you’ll encounter three very different attractions. There’s no missing the austere gray ramparts of Fort Charlotte, which guards the western approaches to Nassau Harbour. Built by Lord Dunmore in 1787–89, during the Napoleonic Wars, and named after the wife of George III, this is the largest fort in the Bahamas. But not one shot was ever fired from here in anger — the only volleys ever launched were part of ceremonial salutes. Life must have been pretty boring for the soldiers as many had the time to carve their names in the stones along the battlements. Guides escort visitors around the interior of the fort as well as through the dungeons, which, thankfully, saw little torture. In fact Fort Charlotte is well regarded by New Providence residents as a shelter during hurricanes.
travel_guides/berlitz2/Bahamas-WhereToGo.txt:Northwest of New Providence, Grand Bahama Island was largely ignored through colonial history and was for a long time a comparative backwater. That it is now the second most popular tourist destination in the Bahamas is all due to the forethought of one man — and a great deal of investment made since 1955. The British had little interest in developing Grand Bahama, but the island lies only 55 miles from the Florida coast, and in the post–World War II period it finally attracted the attention of developers. As the economy of the US grew and Bahamian–US trade increased, a group of businessmen, led by Wallace Groves, saw the potential in the development of Grand Bahama.
```

### 3. To search for both lowercase and uppercase
`grep -i` can be used to make the grep command search for the string, in both uppercase and lowercase.

```
Ayans-MacBook-Pro:written_2 ayan$ grep -i "Without" */*/*
grep: non-fiction/OUP/Abernathy: Is a directory
grep: non-fiction/OUP/Berk: Is a directory
grep: non-fiction/OUP/Castro: Is a directory
grep: non-fiction/OUP/Fletcher: Is a directory
grep: non-fiction/OUP/Kauffman: Is a directory
grep: non-fiction/OUP/Rybczynski: Is a directory
travel_guides/berlitz1/HandRHawaii.txt:        top French restaurant (La Mer), and the serene House Without A Key
travel_guides/berlitz1/HandRHongKong.txt:        summer and at Christmas. If you do arrive without making advance
travel_guides/berlitz1/HandRJerusalem.txt:        room if you’ve arrived without a reservation.
travel_guides/berlitz1/HandRLakeDistrict.txt:        If you arrive in the Lake District without a reservation,
travel_guides/berlitz1/HandRMadrid.txt:        location. Comfortable and affordable It’s usually full but without the
travel_guides/berlitz1/HandRMallorca.txt:        go, it’s not wise to descend on either island without reservations
travel_guides/berlitz1/HistoryDublin.txt:        Christianized — a peaceful process, without a single martyr, which
travel_guides/berlitz1/HistoryEdinburgh.txt:        without a ruler. There were a number of claimants to the throne, among
travel_guides/berlitz1/HistoryEdinburgh.txt:        was bitterly ironic when Elizabeth died without an heir and James,
travel_guides/berlitz1/HistoryEgypt.txt:        Tutankhamun died in mysterious circumstances without an
travel_guides/berlitz1/HistoryFrance.txt:        was not without cost. It took French historians a long time to come to
travel_guides/berlitz1/HistoryIndia.txt:        without direct heir, his state “lapsed” into British hands. If, after
travel_guides/berlitz1/HistoryIndia.txt:        Without giving up demands for self-determination, India
travel_guides/berlitz1/HistoryIndia.txt:        trials without jury and also internment without trial. Popular protest
travel_guides/berlitz1/HistoryIndia.txt:        Allahabad, and without ritual. The mourning crowds, though, ignored his
travel_guides/berlitz1/HistoryIsrael.txt:        positions in Beirut. They forced the PLO out, but without much support
travel_guides/berlitz1/HistoryIstanbul.txt:        sultanate without antagonizing the religious elements within his party.
travel_guides/berlitz1/HistoryItaly.txt:        (1182–1226), pious without being troublesomely militant. His sermons
travel_guides/berlitz1/HistoryItaly.txt:        had existed through most of their history without it and Mussolini had
travel_guides/berlitz1/HistoryJapan.txt:        shrines stretching to the south. In those peaceful years, without
travel_guides/berlitz1/HistoryJapan.txt:        real power. Neither could exist without the other.
travel_guides/berlitz1/HistoryJapan.txt:        a means of winning favor with the Portuguese traders, without
travel_guides/berlitz1/HistoryJapan.txt:        at the end of the country’s century of civil war, Tokugawa was without
travel_guides/berlitz1/HistoryJapan.txt:        Without access to foreign markets, there was no way to counter the rash
travel_guides/berlitz1/HistoryJapan.txt:        Prosperity was not without its own problems: pollution caused by
travel_guides/berlitz1/HistoryLasVegas.txt:        permanent shelters year-round without need to follow wildlife.
travel_guides/berlitz1/HistoryMadeira.txt:        strength, without aid of machinery, carved flat surfaces out of the
travel_guides/berlitz1/HistoryMalaysia.txt:        Johor’s rights in tin exports from Perak, Selangor, and Klang. Without
travel_guides/berlitz1/HistoryMalaysia.txt:        energy to their communities. ) The region was unproductive and without
travel_guides/berlitz1/HistoryMalaysia.txt:        and the Repulse, sailed north. But without air cover, they were spotted
travel_guides/berlitz1/HistoryMallorca.txt:        Balearics, without imposing Islam. But by 848 disturbances in the
travel_guides/berlitz1/IntroEgypt.txt:        some things never change. Just as in ancient times, without the River
travel_guides/berlitz1/IntroFWI.txt:        Saint-Martin (the other side is Dutch) have as much charm — without the
travel_guides/berlitz1/IntroIndia.txt:        This original doctrine, without any sense of Buddha’s
travel_guides/berlitz1/IntroLakeDistrict.txt:        rivers that feed the lakes, so without it, of course, the magnificent
travel_guides/berlitz1/IntroLasVegas.txt:        via a giant pipeline connected to the Colorado River. Without that
```
Over here even the lowercase results can be seen although the main string was 'Without' and not 'without'.

```
Ayans-MacBook-Pro:travel_guides ayan$ grep -i "puerto" */*
berlitz1/HistoryHawaii.txt:        and importing new workers to plant and cultivate them. Puerto Ricans
berlitz1/HistoryJamaica.txt:        or Puerto Rico and, consequently, was poorly protected.
berlitz1/WhatToFWI.txt:        waters off the Bahamas, Puerto Rico, and the Virgin Islands, but the
berlitz1/WhereToMallorca.txt:        glamorous-looking marina of Puerto Punta Portals is not natural but
berlitz2/CanaryIslands-WhatToDo.txt:Fishing: Deep-sea fishing charters for the likes of shark, barracuda, marlin, and tuna are available at Los Cristianos Harbor (Tenerife), Puerto Rico (Gran Canaria), Peurto Calero (Lanzarote) and Corralejo (Fuerteventura).
berlitz2/CanaryIslands-WhatToDo.txt:On Tenerife, Quad Aventura and Tanarán Jeep Safari are both located at Playa de las Américas or Puerto de La Cruz. Miguel’s Jeep-Safaris operate on Gran Canaria.
berlitz2/CanaryIslands-WhatToDo.txt:Surfing: A few beaches have the right conditions for surfing. Playa de Martiánez at Puerto de la Cruz (Tenerife) is very popular and you can also ride the waves at Playa de las Canteras, Las Palmas (Gran Canaria).
berlitz2/CanaryIslands-WhatToDo.txt:Vela Latina: Lateens, old-fashioned Canaries sailing rigs with triangular sails, race against each other on Saturday afternoons and Sunday mornings at Las Palmas and Puerto Rico on Gran Canaria, between April and September.
berlitz2/CanaryIslands-WhatToDo.txt:Carnaval is biggest and best in Santa Cruz and Puerto de la Cruz on Tenerife and in Las Palmas on Gran Canaria, where it has all the razzmatazz of Rio’s Carnaval and the Mardi Gras of New Orleans. Visitors come from all over the world for these events, and hotels are often full, so book well ahead if you plan to visit at this time of year.
berlitz2/CanaryIslands-WhatToDo.txt:Playa San Juan (between Playa de Américas and Los Gigantes) offers Nostramo, an original 1918 schooner; Playa de Américas/Los Cristianos has the only glass bottom catamaran in Puerto Colón: Tropical Delfin. In south Tenerife you can also try Bonadea II (Puerto Colón, dock pantalan 4); Sea Quest (Puerto Colón, dock pantalan 8). 
berlitz2/CanaryIslands-WhatToDo.txt:Pick a banana. A trip to the banana plantation of Bananera El Guanche (see pages 26), outside Puerto de la Cruz, Tenerife, may not initially sound very exciting to a youngster. But the sight of whole banana fists growing wild is a novelty and the easy-to-follow video that precedes the self-guided tour makes learning fun. Adults get a banana liqueur at the end of the tour.
berlitz2/CanaryIslands-WhatToDo.txt:Submarine Trips: see Where To Go for info on these excursions. Puerto Colón, Playa de Américas (Tenerife); Peurto de Mogán (Gran Canaria); and Puerto Calero (Lanzarote).
berlitz2/CanaryIslands-WhatToDo.txt:Puerto de La Cruz (Tenerife Palace): a meal at 8pm followed by a long-established cabaret show at 9:15pm (5,350 ptas, r32.15 per person).
berlitz2/CanaryIslands-WhatToDo.txt:Casino — Playa de las Américas, Hotel Gran Tenerife (open 8pm–4am; entrance 500 ptas, r3.01). Casino Royale — Mare Nostrum Resort, <www.marenostrumresort.com>, (admission with dinner shows only). Casino Taoro — Puerto de la Cruz is the most famous in betting circles (open 8pm to the early hours). Casino Las Palmas — Hotel Santa Catalina, Las Palmas de Gran Canaria (open daily 8pm–4am, until 5am on Friday and Saturday; admission 500 ptas, r3.01). Casino Gran Canaria — Hotel Meliá Tamarindos, Playa de San Agustín, Maspalomas (open daily 8pm–4am; admission 500 ptas, r3.01). Casino de Lanzarote — Puerto del Carmen (gambling machines open daily 11am–4am and gambling hall 8pm–4am.
berlitz2/CanaryIslands-WhereToGo.txt:Tenerife has been welcoming visitors from cold northern climes since the 19th century. However, the focus has changed from the cloudy, green north coast where Puerto de la Cruz was once the favorite resort (it is still enormously popular), to the hot, dry, arid south.
berlitz2/CanaryIslands-WhereToGo.txt:Puerto de la Cruz
berlitz2/CanaryIslands-WhereToGo.txt:Puerto, as this town is often abbreviated to, has neither good beaches nor the abundant sunshine of the south, yet for many travelers it is the most complete resort on the island. It has been attracting convalescing northern Europeans for over a century and it maintains much of its colonial grandeur. The seafront promenade has been quite heavily commercialized but not at all spoiled, and the atmosphere is always lively without being boisterous. The main square, Plaza de Charco, is the hub of both tourist and local life, and its numerous cafés, restaurants, and shops are busy at all hours. Just off the square, the old town around the Puerto Pesquero is remarkably oblivious to change. Among the narrow streets with faded wooden balconies and carved doors are the Casa de Miranda, now a crafts shop and restaurant, and, oldest of all, the Casa de la Real Aduana (Customs House), built in 1620, facing the tiny port.
berlitz2/CanaryIslands-WhereToGo.txt:The problem of Puerto’s lack of a decent beach was brilliantly addressed by the late César Manrique who designed Lago Martiánez, which is open daily 9:45am to 5pm. This 3-hectare (8-acre) complex of tropical lagoons, cascading fountains and sunbathing terraces is cleverly landscaped with lush palms and black-and-white volcanic rocks to fit perfectly into the seafront, where the surf crashes spectacularly against the rocks.
berlitz2/CanaryIslands-WhereToGo.txt:There are numerous places on Tenerife competing for the attention of tourists, but there is one, just to the west of Puerto, that absolutely should not be missed. Loro Parque; (open daily 8:30am–5pm, admission: 2,900 ptas, r17.43) has the world’s largest collection of parrots — more than 300 species and subspecies. It is also home to the most eclectic array of animals including gorillas, chimpanzees, tigers, jaguars, alligators, sea-lions, dolphins and numerous other creatures that are exhibited in carefully and creatively, designed spaces. Look also for the underwater world of the aquarium and shark tunnel, and the newest, and undoubtedly most inventive display. The Planet Penguin, the largest Penguinarium in the world, covers 3,900 square m (nearly 1 acre) and has been created as a natural habitat for these engaging creatures. The temperature of their iceberg is kept at between -2º and 2º C (28º–36º F) with 12 tons of artificial snow falling on it daily through openings in the roof. The surrounding sea is chilled to 10º C (50º F). Visitors are conveyed around on a moving walkway that allows the King, Gentoo and Rockhopper penguins to be seen cavorting on land and in the water. Look also for the dolphin, sea lion, and parrot shows, and animal feedings.
```

### 4. To Count the Number of Matches
`grep -c` can be used to get the number of times a string appears in a file.

```
Ayans-MacBook-Pro:travel_guides ayan$ grep -c "and" */*
berlitz1/HandRHawaii.txt:63
berlitz1/HandRHongKong.txt:4
berlitz1/HandRIbiza.txt:3
berlitz1/HandRIsrael.txt:110
berlitz1/HandRIstanbul.txt:2
berlitz1/HandRJamaica.txt:128
berlitz1/HandRJerusalem.txt:4
berlitz1/HandRLakeDistrict.txt:10
berlitz1/HandRLasVegas.txt:8
berlitz1/HandRLisbon.txt:5
berlitz1/HandRLosAngeles.txt:8
berlitz1/HandRMadeira.txt:9
berlitz1/HandRMadrid.txt:53
berlitz1/HandRMallorca.txt:7
berlitz1/HistoryDublin.txt:105
berlitz1/HistoryEdinburgh.txt:145
berlitz1/HistoryEgypt.txt:97
berlitz1/HistoryFWI.txt:86
berlitz1/HistoryFrance.txt:193
berlitz1/HistoryGreek.txt:136
berlitz1/HistoryHawaii.txt:103
berlitz1/HistoryHongKong.txt:72
berlitz1/HistoryIbiza.txt:82
berlitz1/HistoryIndia.txt:290
berlitz1/HistoryIsrael.txt:98
berlitz1/HistoryIstanbul.txt:140
berlitz1/HistoryItaly.txt:256
berlitz1/HistoryJamaica.txt:99
berlitz1/HistoryJapan.txt:203
berlitz1/HistoryJerusalem.txt:82
berlitz1/HistoryLakeDistrict.txt:93
berlitz1/HistoryLasVegas.txt:77
berlitz1/HistoryMadeira.txt:73
berlitz1/HistoryMadrid.txt:53
berlitz1/HistoryMalaysia.txt:192
berlitz1/HistoryMallorca.txt:87
berlitz1/IntroDublin.txt:53
berlitz1/IntroEdinburgh.txt:49
berlitz1/IntroEgypt.txt:50
berlitz1/IntroFWI.txt:48
berlitz1/IntroFrance.txt:81
berlitz1/IntroGreek.txt:67
berlitz1/IntroHongKong.txt:36
berlitz1/IntroIbiza.txt:39
berlitz1/IntroIndia.txt:120
berlitz1/IntroIsrael.txt:33
berlitz1/IntroIstanbul.txt:36
berlitz1/IntroItaly.txt:74
berlitz1/IntroJamaica.txt:73
berlitz1/IntroJapan.txt:83
berlitz1/IntroJerusalem.txt:58
berlitz1/IntroLakeDistrict.txt:83
berlitz1/IntroLasVegas.txt:62
```
The number of occurences of the word 'and' are displayed next to each filename.

```
Ayans-MacBook-Pro:travel_guides ayan$ grep -c "with" */*
berlitz1/HandRHawaii.txt:31
berlitz1/HandRHongKong.txt:3
berlitz1/HandRIbiza.txt:1
berlitz1/HandRIsrael.txt:41
berlitz1/HandRIstanbul.txt:1
berlitz1/HandRJamaica.txt:58
berlitz1/HandRJerusalem.txt:3
berlitz1/HandRLakeDistrict.txt:2
berlitz1/HandRLasVegas.txt:2
berlitz1/HandRLisbon.txt:1
berlitz1/HandRLosAngeles.txt:4
berlitz1/HandRMadeira.txt:1
berlitz1/HandRMadrid.txt:13
berlitz1/HandRMallorca.txt:3
berlitz1/HistoryDublin.txt:16
berlitz1/HistoryEdinburgh.txt:18
berlitz1/HistoryEgypt.txt:23
berlitz1/HistoryFWI.txt:12
berlitz1/HistoryFrance.txt:52
berlitz1/HistoryGreek.txt:12
berlitz1/HistoryHawaii.txt:13
berlitz1/HistoryHongKong.txt:17
berlitz1/HistoryIbiza.txt:11
berlitz1/HistoryIndia.txt:64
berlitz1/HistoryIsrael.txt:17
berlitz1/HistoryIstanbul.txt:24
berlitz1/HistoryItaly.txt:65
berlitz1/HistoryJamaica.txt:17
berlitz1/HistoryJapan.txt:48
berlitz1/HistoryJerusalem.txt:24
berlitz1/HistoryLakeDistrict.txt:8
berlitz1/HistoryLasVegas.txt:20
berlitz1/HistoryMadeira.txt:10
berlitz1/HistoryMadrid.txt:9
berlitz1/HistoryMalaysia.txt:45
berlitz1/HistoryMallorca.txt:12
berlitz1/IntroDublin.txt:7
berlitz1/IntroEdinburgh.txt:14
berlitz1/IntroEgypt.txt:8
berlitz1/IntroFWI.txt:10
berlitz1/IntroFrance.txt:7
berlitz1/IntroGreek.txt:12
berlitz1/IntroHongKong.txt:11
berlitz1/IntroIbiza.txt:9
berlitz1/IntroIndia.txt:26
berlitz1/IntroIsrael.txt:3
berlitz1/IntroIstanbul.txt:7
berlitz1/IntroItaly.txt:12
berlitz1/IntroJamaica.txt:14
berlitz1/IntroJapan.txt:16
berlitz1/IntroJerusalem.txt:12
berlitz1/IntroLakeDistrict.txt:9
berlitz1/IntroLasVegas.txt:11
berlitz1/IntroLosAngeles.txt:12
berlitz1/IntroMadeira.txt:9
berlitz1/IntroMadrid.txt:9
berlitz1/IntroMalaysia.txt:13
berlitz1/IntroMallorca.txt:8
berlitz1/JungleMalaysia.txt:6
berlitz1/WhatToDublin.txt:19
berlitz1/WhatToEdinburgh.txt:28
berlitz1/WhatToEgypt.txt:33
berlitz1/WhatToFWI.txt:31
berlitz1/WhatToFrance.txt:0
berlitz1/WhatToGreek.txt:18
berlitz1/WhatToHawaii.txt:3
berlitz1/WhatToHongKong.txt:22
berlitz1/WhatToIbiza.txt:50
berlitz1/WhatToIndia.txt:22
berlitz1/WhatToIsrael.txt:13
berlitz1/WhatToIstanbul.txt:49
berlitz1/WhatToItaly.txt:16
berlitz1/WhatToJamaica.txt:108
berlitz1/WhatToJapan.txt:40
berlitz1/WhatToLakeDistrict.txt:16
berlitz1/WhatToLasVegas.txt:52
```

### Additional Info
By combining commands together, such as using `-r` with `-i` we can go through the subdirectories of `non-fiction` without getting an error. We can also use `less` with these grep commands to scroll through the large amount of results with ease.
