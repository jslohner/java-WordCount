# Project Top Word Counts in A String of Text

A student that completes this project shows that they can:

* Craft and use for loops
* Craft and use Java conditionals, branching, including if-then, if-then-else, and switch statements
* Craft and manipulate Collections
* Craft and manipulate ArraysList Collections
* Craft and manipulate HashMap Collections

## Introduction

Reading in some text and counting word frequencies is a very common Java interview question. So, let's practice that!

## Instructions

Below, the ***United Nation’s Declaration of Human Rights*** is provided as a string. The sections have been combined into one string for ease of parsing that string. Also, some punctation has been removed, again to ease in parsing the string. Make sure when you copy the string, no line breaks are copied!

`Preamble Whereas recognition of the inherent dignity and of the equal and inalienable rights of all members of the human family is the foundation of freedom, justice and peace in the world,  Whereas disregard and contempt for human rights have resulted in barbarous acts which have outraged the conscience of mankind, and the advent of a world in which human beings shall enjoy freedom of speech and belief and freedom from fear and want has been proclaimed as the highest aspiration of the common people,  Whereas it is essential, if man is not to be compelled to have recourse, as a last resort, to rebellion against tyranny and oppression, that human rights should be protected by the rule of law,  Whereas it is essential to promote the development of friendly relations between nations,  Whereas the peoples of the United Nations have in the Charter reaffirmed their faith in fundamental human rights, in the dignity and worth of the human person and in the equal rights of men and women and have determined to promote social progress and better standards of life in larger freedom,  Whereas Member States have pledged themselves to achieve, in co-operation with the United Nations, the promotion of universal respect for and observance of human rights and fundamental freedoms,  Whereas a common understanding of these rights and freedoms is of the greatest importance for the full realization of this pledge,  Now, Therefore THE GENERAL ASSEMBLY proclaims THIS UNIVERSAL DECLARATION OF HUMAN RIGHTS as a common standard of achievement for all peoples and all nations, to the end that every individual and every organ of society, keeping this Declaration constantly in mind, shall strive by teaching and education to promote respect for these rights and freedoms and by progressive measures, national and international, to secure their universal and effective recognition and observance, both among the peoples of Member States themselves and among the peoples of territories under their jurisdiction.   Article 1.   All human beings are born free and equal in dignity and rights. They are endowed with reason and conscience and should act towards one another in a spirit of brotherhood.  Article 2.   Everyone is entitled to all the rights and freedoms set forth in this Declaration, without distinction of any kind, such as race, colour, sex, language, religion, political or other opinion, national or social origin, property, birth or other status. Furthermore, no distinction shall be made on the basis of the political, jurisdictional or international status of the country or territory to which a person belongs, whether it be independent, trust, non-self-governing or under any other limitation of sovereignty.  Article 3.   Everyone has the right to life, liberty and security of person.  Article 4.   No one shall be held in slavery or servitude; slavery and the slave trade shall be prohibited in all their forms.  Article 5.   No one shall be subjected to torture or to cruel, inhuman or degrading treatment or punishment.  Article 6.   Everyone has the right to recognition everywhere as a person before the law.  Article 7.   All are equal before the law and are entitled without any discrimination to equal protection of the law. All are entitled to equal protection against any discrimination in violation of this Declaration and against any incitement to such discrimination.  Article 8.   Everyone has the right to an effective remedy by the competent national tribunals for acts violating the fundamental rights granted him by the constitution or by law.  Article 9.   No one shall be subjected to arbitrary arrest, detention or exile.  Article 10.   Everyone is entitled in full equality to a fair and public hearing by an independent and impartial tribunal, in the determination of his rights and obligations and of any criminal charge against him.  Article 11.   (1) Everyone charged with a penal offence has the right to be presumed innocent until proved guilty according to law in a public trial at which he has had all the guarantees necessary for his defence. (2) No one shall be held guilty of any penal offence on account of any act or omission which did not constitute a penal offence, under national or international law, at the time when it was committed. Nor shall a heavier penalty be imposed than the one that was applicable at the time the penal offence was committed.  Article 12.   No one shall be subjected to arbitrary interference with his privacy, family, home or correspondence, nor to attacks upon his honour and reputation. Everyone has the right to the protection of the law against such interference or attacks.  Article 13.   (1) Everyone has the right to freedom of movement and residence within the borders of each state. (2) Everyone has the right to leave any country, including his own, and to return to his country.  Article 14.   (1) Everyone has the right to seek and to enjoy in other countries asylum from persecution. (2) This right may not be invoked in the case of prosecutions genuinely arising from non-political crimes or from acts contrary to the purposes and principles of the United Nations.  Article 15.   (1) Everyone has the right to a nationality. (2) No one shall be arbitrarily deprived of his nationality nor denied the right to change his nationality.  Article 16.   (1) Men and women of full age, without any limitation due to race, nationality or religion, have the right to marry and to found a family. They are entitled to equal rights as to marriage, during marriage and at its dissolution. (2) Marriage shall be entered into only with the free and full consent of the intending spouses. (3) The family is the natural and fundamental group unit of society and is entitled to protection by society and the State.  Article 17.   (1) Everyone has the right to own property alone as well as in association with others. (2) No one shall be arbitrarily deprived of his property.  Article 18.   Everyone has the right to freedom of thought, conscience and religion; this right includes freedom to change his religion or belief, and freedom, either alone or in community with others and in public or private, to manifest his religion or belief in teaching, practice, worship and observance.  Article 19.   Everyone has the right to freedom of opinion and expression; this right includes freedom to hold opinions without interference and to seek, receive and impart information and ideas through any media and regardless of frontiers.  Article 20.   (1) Everyone has the right to freedom of peaceful assembly and association. (2) No one may be compelled to belong to an association.  Article 21.   (1) Everyone has the right to take part in the government of his country, directly or through freely chosen representatives. (2) Everyone has the right of equal access to public service in his country. (3) The will of the people shall be the basis of the authority of government; this will shall be expressed in periodic and genuine elections which shall be by universal and equal suffrage and shall be held by secret vote or by equivalent free voting procedures.  Article 22.   Everyone, as a member of society, has the right to social security and is entitled to realization, through national effort and international co-operation and in accordance with the organization and resources of each State, of the economic, social and cultural rights indispensable for his dignity and the free development of his personality.  Article 23.   (1) Everyone has the right to work, to free choice of employment, to just and favourable conditions of work and to protection against unemployment. (2) Everyone, without any discrimination, has the right to equal pay for equal work. (3) Everyone who works has the right to just and favourable remuneration ensuring for himself and his family an existence worthy of human dignity, and supplemented, if necessary, by other means of social protection. (4) Everyone has the right to form and to join trade unions for the protection of his interests.  Article 24.   Everyone has the right to rest and leisure, including reasonable limitation of working hours and periodic holidays with pay.  Article 25.   (1) Everyone has the right to a standard of living adequate for the health and well-being of himself and of his family, including food, clothing, housing and medical care and necessary social services, and the right to security in the event of unemployment, sickness, disability, widowhood, old age or other lack of livelihood in circumstances beyond his control. (2) Motherhood and childhood are entitled to special care and assistance. All children, whether born in or out of wedlock, shall enjoy the same social protection.  Article 26.   (1) Everyone has the right to education. Education shall be free, at least in the elementary and fundamental stages. Elementary education shall be compulsory. Technical and professional education shall be made generally available and higher education shall be equally accessible to all on the basis of merit. (2) Education shall be directed to the full development of the human personality and to the strengthening of respect for human rights and fundamental freedoms. It shall promote understanding, tolerance and friendship among all nations, racial or religious groups, and shall further the activities of the United Nations for the maintenance of peace. (3) Parents have a prior right to choose the kind of education that shall be given to their children.  Article 27.   (1) Everyone has the right freely to participate in the cultural life of the community, to enjoy the arts and to share in scientific advancement and its benefits. (2) Everyone has the right to the protection of the moral and material interests resulting from any scientific, literary or artistic production of which he is the author.  Article 28.   Everyone is entitled to a social and international order in which the rights and freedoms set forth in this Declaration can be fully realized.  Article 29.   (1) Everyone has duties to the community in which alone the free and full development of his personality is possible. (2) In the exercise of his rights and freedoms, everyone shall be subject only to such limitations as are determined by law solely for the purpose of securing due recognition and respect for the rights and freedoms of others and of meeting the just requirements of morality, public order and the general welfare in a democratic society. (3) These rights and freedoms may in no case be exercised contrary to the purposes and principles of the United Nations.  Article 30.   Nothing in this Declaration may be interpreted as implying for any State, group or person any right to engage in any activity or to perform any act aimed at the destruction of any of the rights and freedoms set forth herein.`

* [ ] Please fork and clone this repository. This repository does not have a starter project, so create one inside of the cloned repository folder. Regularly commit and push your code as appropriate.

* [ ] Set the above to be a String in Java, so something like `String unText = "...";`

* [ ] From this string, make a HashMap of each unique word and the frequency it appears in the text.
  * A word is delimited by a space or punctuation mark(s).
  * The spaces and punctuation marks do NOT appear in the word list.
  * The word list is NOT case sensitive: Lambda / lambda will count as the same word.
  * Words such as co-operation that contain a hyphen are considered one word.
  * A hyphen alone does not separate words. Numbers count as one word, so 23 is a word.

* [ ] Print to the console the top 50 appearing words along with their counts.

  * Remember that HashMaps are not sorted nor easily sortable. You could convert the HashMap to an array list and then sort the array list. Alternatively, you can find the most common word, print it, remove it, and repeat the process.

Note:

Below are two snippets of code you might find useful for this afternoon. Of course if you do not find them useful please ignore. You are NOT required to use this code.

```JAVA
// remove all remaining punctuation from the string
myStr.replaceAll("[[\\.\\?\\!\\,\\;\\:\\{\\}\\(\\)\\']]", "");

// split a string into words
`String[] words = myStr.split(" +");`
```

Output should be something like

```TEXT
Top 50 words

Common Word <THE> occurs 120 times
Common Word <AND> occurs 106 times
Common Word <OF> occurs 90 times
Common Word <TO> occurs 83 times
Common Word <IN> occurs 43 times
Common Word <RIGHT> occurs 33 times
Common Word <BE> occurs 31 times
Common Word <OR> occurs 30 times
Common Word <EVERYONE> occurs 30 times
Common Word <ARTICLE> occurs 30 times
Common Word <HAS> occurs 28 times
Common Word <SHALL> occurs 27 times
Common Word <RIGHTS> occurs 21 times
Common Word <HIS> occurs 21 times
Common Word <A> occurs 19 times
Common Word <ANY> occurs 18 times
Common Word <FOR> occurs 17 times
Common Word <1> occurs 14 times
Common Word <2> occurs 14 times
Common Word <BY> occurs 13 times
Common Word <IS> occurs 13 times
Common Word <HUMAN> occurs 12 times
Common Word <ALL> occurs 12 times
Common Word <AS> occurs 11 times
Common Word <EQUAL> occurs 11 times
Common Word <FREEDOM> occurs 11 times
Common Word <THIS> occurs 11 times
Common Word <FREEDOMS> occurs 10 times
Common Word <NO> occurs 10 times
Common Word <ONE> occurs 10 times
Common Word <WITH> occurs 9 times
Common Word <WHICH> occurs 9 times
Common Word <LAW> occurs 9 times
Common Word <PROTECTION> occurs 9 times
Common Word <ENTITLED> occurs 9 times
Common Word <NATIONS> occurs 8 times
Common Word <HAVE> occurs 8 times
Common Word <SOCIAL> occurs 8 times
Common Word <ARE> occurs 8 times
Common Word <EDUCATION> occurs 8 times
Common Word <WHEREAS> occurs 7 times
Common Word <FREE> occurs 7 times
Common Word <3> occurs 6 times
Common Word <AT> occurs 6 times
Common Word <FAMILY> occurs 6 times
Common Word <DECLARATION> occurs 6 times
Common Word <FUNDAMENTAL> occurs 6 times
Common Word <OTHER> occurs 6 times
Common Word <FULL> occurs 6 times
Common Word <AGAINST> occurs 6 times
```

## Stretch Goals

* [ ] Print to the console the top 50 appearing words alphabetically. Do include their counts.

Output should be something like

```TEXT
Top 50 words Alphabetically

Common Word <1> occurs 14 times
Common Word <2> occurs 14 times
Common Word <3> occurs 6 times
Common Word <A> occurs 19 times
Common Word <AGAINST> occurs 6 times
Common Word <ALL> occurs 12 times
Common Word <AND> occurs 106 times
Common Word <ANY> occurs 18 times
Common Word <ARE> occurs 8 times
Common Word <ARTICLE> occurs 30 times
Common Word <AS> occurs 11 times
Common Word <AT> occurs 6 times
Common Word <BE> occurs 31 times
Common Word <BY> occurs 13 times
Common Word <DECLARATION> occurs 6 times
Common Word <EDUCATION> occurs 8 times
Common Word <ENTITLED> occurs 9 times
Common Word <EQUAL> occurs 11 times
Common Word <EVERYONE> occurs 30 times
Common Word <FAMILY> occurs 6 times
Common Word <FOR> occurs 17 times
Common Word <FREE> occurs 7 times
Common Word <FREEDOM> occurs 11 times
Common Word <FREEDOMS> occurs 10 times
Common Word <FULL> occurs 6 times
Common Word <FUNDAMENTAL> occurs 6 times
Common Word <HAS> occurs 28 times
Common Word <HAVE> occurs 8 times
Common Word <HIS> occurs 21 times
Common Word <HUMAN> occurs 12 times
Common Word <IN> occurs 43 times
Common Word <IS> occurs 13 times
Common Word <LAW> occurs 9 times
Common Word <NATIONS> occurs 8 times
Common Word <NO> occurs 10 times
Common Word <OF> occurs 90 times
Common Word <ONE> occurs 10 times
Common Word <OR> occurs 30 times
Common Word <OTHER> occurs 6 times
Common Word <PROTECTION> occurs 9 times
Common Word <RIGHT> occurs 33 times
Common Word <RIGHTS> occurs 21 times
Common Word <SHALL> occurs 27 times
Common Word <SOCIAL> occurs 8 times
Common Word <THE> occurs 120 times
Common Word <THIS> occurs 11 times
Common Word <TO> occurs 83 times
Common Word <WHEREAS> occurs 7 times
Common Word <WHICH> occurs 9 times
Common Word <WITH> occurs 9 times
```
