# Harmful Content Classification Criteria
We classified potentially harmful content in Ethereum transactions into six categories: **Privacy Violation**, **Sexual Content**, **Discrimination**, **On-chain Crime**, **Personal Threat**, and **Child Maltreatment**.
Below, we provide detailed classification criteria and corresponding cases.

## 1. Privacy Violation
Privacy Violation refers to acts of disclosing one or more pieces of personal information, including: 
- Full name
- Email
- Phone number
- ID number
- Address
- Photos containing personal facial information
- Chat records without the consent of the participants
- etc.

Note that public content, such as news, declarations, and advertisements, should not be considered as privacy violations.

Examples (anonymized):
```
J**** J****** - **********@gmail.com
```

## 2. Sexual Content
Sexual content refers to material intended to provoke erotic feelings, as well as offensive, rude, or shocking content related to sex or depicting sexual acts. Specifically, the following content will be considered as sexual content:
- Pornography
- Sex services
- Obscene insults related to sex
- Images or videos containing private body parts

Example (anonymized): 
```
Sex dating in Australiа | Girls fоr sex in Australia: https://onlineuniversalwork.com/***************
```

## 3. Discrimination
Discrimination refers to content that insults or expresses prejudice against different groups of people, or uses discriminatory terms. 

Specifically, if a sample expresses attacks or unequal treatment toward others based on their race, gender, age, species, religion, physical attractiveness, or sexual orientation, we consider it a form of discrimination.
Additionally, we use the [Hatebase](https://hatebase.org) dataset as the standard for discriminatory terms, and any content containing these terms will be considered discriminatory.
Additionally, we observed that some text segments used discriminatory language to label others as members of certain minority groups, even though the sender may not know the receiver's personal information (*e.g.*, sexual orientation). Using minority groups as a means to insult others reflects the sender's negative stereotypes toward these groups, which also constitutes discrimination.

Example (anonymized): 
```
fucken fa**ot
```

## 4. On-chain Crime
The *United Nations Convention Against Transnational Organized Crime* defines a wide range of illegal activities, including:
- Money laundering
- Drug trafficking
- Terrorism
- Smuggling
- Human trafficking
- Manufacture and trafficking of firearms
- Corruption
- Other serious crimes (*i.e.*, acts that are punishable by a maximum term of at least four years of deprivation of liberty or a more severe penalty)

We use this convention as the standard for detecting on-chain crimes. Any content involving the commission of criminal activities, encouraging crimes, or teaching criminal methods is categorized under this type.

Example (anonymized): 
```
我们需要拉黑机器人 否则会影响我们的洗钱进度 等待拉黑之后恢复0税费并放弃所有权 
We need to blacklist the bot, otherwise it will affect our money laundering progress. Once blacklisted, we will restore a 0% tax rate and relinquish ownership.
```
<!-- - Wilt u online wiet of hasj kopen in Nederland en België? Zoek dan niet verder, bij http://\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*/ bent u aan het juiste adres. (Do you want to buy weed or hash online in the Netherlands and Belgium? Look no further, at http://\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*/ you’ve come to the right place.) -->

## 5. Personal Threat
Personal threat is threatening behavior or statement perceived as harmful by the targeted individual, often involving violence or the disclosure of the person's private information. 

Example (anonymized): 
```
GOOD NEWS! I HAVE GOT YOUR SOCIAL IDENTITY.  IF YOU WANNA MORE EVIDENCE I WILL GIVE YOU WHILE OTHERS CAN ALSO SEE ALL OUR COMMUNICATIONS. YOU SAID YOU WILL GIVE ME A PERSONAL GIFT. I WOULD LIKE 32 ETH.
```

## 6. Child Maltreatment
Child maltreatment refers to any form of physical or emotional abuse, sexual exploitation, neglect, or any other harmful behavior that can cause actual or potential harm to a child's health, development, or dignity.

Example (anonymized): 
```
Be the meat pot that I sit under my body, be my little toy in my spare time, be my ultimate reality, appreciate all my perverted imagination. wrote by my dear daughter **. uploaded by father ****@20190214
```