# Amazon EC2 Windows Server AMIs for STIG compliance<a name="ami-windows-stig"></a>

Security Technical Implementation Guides \(STIGs\) are the configuration standards created by the Defense Information Systems Agency \(DISA\) to secure information systems and software\. To make your systems compliant with STIG standards, you must install, configure, and test a variety of security settings\. Amazon EC2 Windows Server AMIs for STIG Compliance are pre\-configured with over 160 required security settings\. STIG\-compliant operating systems include Windows Server 2012 R2, Windows Server 2016, and Windows Server 2019\. The STIG\-compliant AMIs include updated Department of Defense \(DoD\) certificates to help you get started and achieve STIG compliance\. There are no additional charges for using STIG\-compliant AMIs\.

Amazon EC2 Windows Server AMIs for STIG compliance are available in all public AWS and GovCloud Regions\. You can launch instances from these AMIs directly from the Amazon EC2 console\. They are billed using standard Windows pricing\.

The STIG\-compliant Amazon EC2 AMIs for Windows Server can be found in the Community AMIs when you create an instance\. The AMI names are as follows:

**Note**  
The date suffix for the AMI \(*YYYY\.MM\.DD*\) is the date on which the latest version was created\. You can search for the version without the date suffix\.
+ Windows\_Server\-2019\-English\-STIG\-Full\-*YYYY\.MM\.DD*
+ Windows\_Server\-2019\-English\-STIG\-Core\-*YYYY\.MM\.DD*
+ Windows\_Server\-2016\-English\-STIG\-Full\-*YYYY\.MM\.DD*
+ Windows\_Server\-2016\-English\-STIG\-Core\-*YYYY\.MM\.DD*
+ Windows\_Server\-2012\-R2\-English\-STIG\-Full\-*YYYY\.MM\.DD*
+ Windows\_Server\-2012\-R2\-English\-STIG\-Core\-*YYYY\.MM\.DD*

**Compliance levels**
+ **High \(Category I\) **

  The most severe risk\. Includes any vulnerability that can result in loss of confidentiality, availability, or integrity\.
+ **Medium \(Category II\) **

  Includes any vulnerability that could result in loss of confidentiality, availability, or integrity but where the risks could be mitigated\.
+ **Low \(Category III\) **

  Includes any vulnerability that degrades measures to protect against loss of confidentiality, availability, or integrity\.

The following sections show the STIGs that have been applied to Windows Operating Systems and components\.

**Topics**
+ [Core and base operating systems](#base-os-stig)
+ [Microsoft \.NET Framework 4\.0 STIG V2 Release 1](#dotnet-os-stig)
+ [Windows Firewall STIG V1 Release 7](#windows-firewall-stig)
+ [Internet Explorer \(IE\) 11 STIG V1 Release 19](#ie-os-stig)
+ [Version history](#stig-version-history)

## Core and base operating systems<a name="base-os-stig"></a>

STIG\-compliant Amazon EC2 AMIs are designed for use as standalone servers, and have the highest level of STIG settings applied \(Category 1\)\. Each compliance level includes all STIG settings from lower levels, which means that the highest level has all applicable settings from all levels\.

Some STIG settings are not automatically applied\. This can be due to technical limitations – for instance, the STIG setting might not be applicable for standalone servers\. Organization\-specific policies can also prevent automatic application of STIG settings, such as a requirement for administrators to review document settings\. For more details about which STIGs are applied to Amazon EC2 Windows AMIs, you can download our [spreadsheet](https://aws-windows-downloads-us-west-1.s3.us-west-1.amazonaws.com/STIG/Win+STIG.xlsx)\.

For a complete list of Windows STIGs, see the [STIGs Document Library](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=windows)\. For information about how to view the complete list, see [SRG / STIG Tools](https://public.cyber.mil/stigs/srg-stig-tools/)\.

### Windows Server 2019 STIG V2 Release 2<a name="win-server-2019"></a>

All of the following STIG settings for Windows operating systems are applied:
+ **Windows\\Low**

  V\-205691, V\-205819, V\-205858, V\-205859, V\-205860, V\-205870, V\-205871, and V\-205923
+ **Windows\\Medium**

  V\-205625, V\-205626, V\-205627, V\-205629, V\-205630, V\-205633, V\-205634, V\-205635, V\-205636, V\-205637, V\-205638, V\-205639, V\-205643, V\-205644, V\-205648, V\-205649, V\-205650, V\-205651, V\-205652, V\-205655, V\-205656, V\-205659, V\-205660, V\-205662, V\-205671, V\-205672, V\-205673, V\-205675, V\-205676, V\-205678, V\-205679, V\-205680, V\-205681, V\-205682, V\-205683, V\-205684, V\-205685, V\-205686, V\-205687, V\-205688, V\-205689, V\-205690, V\-205692, V\-205693, V\-205694, V\-205697, V\-205698, V\-205708, V\-205709, V\-205712, V\-205714, V\-205716, V\-205717, V\-205718, V\-205719, V\-205720, V\-205722, V\-205729, V\-205730, V\-205733, V\-205747, V\-205751, V\-205752, V\-205754, V\-205756, V\-205758, V\-205759, V\-205760, V\-205761, V\-205762, V\-205764, V\-205765, V\-205766, V\-205767, V\-205768, V\-205769, V\-205770, V\-205771, V\-205772, V\-205773, V\-205774, V\-205775, V\-205776, V\-205777, V\-205778, V\-205779, V\-205780, V\-205781, V\-205782, V\-205783, V\-205784, V\-205795, V\-205796, V\-205797, V\-205798, V\-205801, V\-205808, V\-205809, V\-205810, V\-205811, V\-205812, V\-205813, V\-205814, V\-205815, V\-205816, V\-205817, V\-205821, V\-205822, V\-205823, V\-205824, V\-205825, V\-205826, V\-205827, V\-205828, V\-205830, V\-205831, V\-205832, V\-205833, V\-205834, V\-205835, V\-205836, V\-205837, V\-205838, V\-205839, V\-205840, V\-205841, V\-205861, V\-205863, V\-205865, V\-205866, V\-205867, V\-205868, V\-205869, V\-205872, V\-205873, V\-205874, V\-205878, V\-205879, V\-205880, V\-205881, V\-205889, V\-205891, V\-205905, V\-205911, V\-205912, V\-205915, V\-205916, V\-205917, V\-205918, V\-205920, V\-205921, V\-205922, V\-205924, V\-205925, and V\-236001
+ **Windows\\High**

  V\-205653, V\-205654, V\-205711, V\-205713, V\-205724, V\-205725, V\-205757, V\-205802, V\-205804, V\-205805, V\-205806, V\-205849, V\-205908, V\-205913, V\-205914, and V\-205919

### Windows Server 2016 STIG V2 Release 2<a name="win-server-2016"></a>

All of the following STIG settings for Windows operating systems are applied:
+ **Windows\\Low**

  V\-224916, V\-224917, V\-224918, V\-224919, V\-224931, V\-224942, and V\-225060
+ **Windows\\Medium**

  V\-224850, V\-224852, V\-224853, V\-224854, V\-224855, V\-224856, V\-224857, V\-224858, V\-224859, V\-224866, V\-224867, V\-224868, V\-224869, V\-224870, V\-224871, V\-224872, V\-224873, V\-224881, V\-224882, V\-224883, V\-224884, V\-224885, V\-224886, V\-224887, V\-224888, V\-224889, V\-224890, V\-224891, V\-224892, V\-224893, V\-224894, V\-224895, V\-224896, V\-224897, V\-224898, V\-224899, V\-224900, V\-224901, V\-224902, V\-224903, V\-224904, V\-224905, V\-224906, V\-224907, V\-224908, V\-224909, V\-224910, V\-224911, V\-224912, V\-224913, V\-224914, V\-224915, V\-224920, V\-224922, V\-224924, V\-224925, V\-224926, V\-224927, V\-224928, V\-224929, V\-224930, V\-224935, V\-224936, V\-224937, V\-224938, V\-224939, V\-224940, V\-224941, V\-224943, V\-224944, V\-224945, V\-224946, V\-224947, V\-224948, V\-224949, V\-224951, V\-224952, V\-224953, V\-224955, V\-224956, V\-224957, V\-224959, V\-224960, V\-224962, V\-224963, V\-225010, V\-225013, V\-225014, V\-225015, V\-225016, V\-225017, V\-225018, V\-225019, V\-225021, V\-225022, V\-225023, V\-225024, V\-225028, V\-225029, V\-225030, V\-225031, V\-225032, V\-225033, V\-225034, V\-225035, V\-225038, V\-225039, V\-225040, V\-225041, V\-225042, V\-225043, V\-225047, V\-225049, V\-225050, V\-225051, V\-225052, V\-225055, V\-225056, V\-225057, V\-225058, V\-225061, V\-225062, V\-225063, V\-225064, V\-225065, V\-225066, V\-225067, V\-225068, V\-225069, V\-225072, V\-225073, V\-225074, V\-225076, V\-225078, V\-225080, V\-225081, V\-225082, V\-225083, V\-225084, V\-225086, V\-225087, V\-225088, V\-225089, V\-225092, V\-225093, and V\-236000
+ **Windows\\High**

  V\-224874, V\-224932, V\-224933, V\-224934, V\-224954, V\-224958, V\-224961, V\-225025, V\-225044, V\-225045, V\-225046, V\-225048, V\-225053, V\-225054, and V\-225079

### Windows Server 2012 R2 STIG V3 Release 2<a name="win-server-2012-R2"></a>

All of the following STIG settings for Windows operating systems are applied:
+ **Windows\\Low**

  V\-225537, V\-225536, V\-225526, V\-225525, V\-225514, V\-225511, V\-225490, V\-225489, V\-225488, V\-225487, V\-225485, V\-225484, V\-225483, V\-225482, V\-225481, V\-225480, V\-225479, V\-225476, V\-225473, V\-225468, V\-225462, V\-225460, V\-225459, V\-225412, V\-225394, V\-225392, V\-225376, V\-225363, V\-225362, V\-225360, V\-225359, V\-225358, V\-225357, V\-225355, V\-225343, V\-225342, V\-225336, V\-225335, V\-225334, V\-225333, V\-225332, V\-225331, V\-225330, V\-225328, V\-225327, V\-225324, V\-225319, V\-225318, and V\-225250
+ **Windows\\Medium**

  V\-225574, V\-225573, V\-225572, V\-225571, V\-225570, V\-225569, V\-225568, V\-225567, V\-225566, V\-225565, V\-225564, V\-225563, V\-225562, V\-225561, V\-225560, V\-225559, V\-225558, V\-225557, V\-225555, V\-225554, V\-225553, V\-225551, V\-225550, V\-225549, V\-225548, V\-225546, V\-225545, V\-225544, V\-225543, V\-225542, V\-225541, V\-225540, V\-225539, V\-225538, V\-225535, V\-225534, V\-225533, V\-225532, V\-225531, V\-225530, V\-225529, V\-225528, V\-225527, V\-225524, V\-225523, V\-225522, V\-225521, V\-225520, V\-225519, V\-225518, V\-225517, V\-225516, V\-225515, V\-225513, V\-225510, V\-225509, V\-225508, V\-225506, V\-225504, V\-225503, V\-225502, V\-225501, V\-225500, V\-225494, V\-225486, V\-225478, V\-225477, V\-225475, V\-225474, V\-225472, V\-225471, V\-225470, V\-225469, V\-225464, V\-225463, V\-225461, V\-225458, V\-225457, V\-225456, V\-225455, V\-225454, V\-225453, V\-225452, V\-225448, V\-225443, V\-225442, V\-225441, V\-225415, V\-225414, V\-225413, V\-225411, V\-225410, V\-225409, V\-225408, V\-225407, V\-225406, V\-225405, V\-225404, V\-225402, V\-225401, V\-225400, V\-225398, V\-225397, V\-225395, V\-225393, V\-225391, V\-225389, V\-225386, V\-225385, V\-225384, V\-225383, V\-225382, V\-225381, V\-225380, V\-225379, V\-225378, V\-225377, V\-225375, V\-225374, V\-225373, V\-225372, V\-225371, V\-225370, V\-225369, V\-225368, V\-225367, V\-225356, V\-225353, V\-225352, V\-225351, V\-225350, V\-225349, V\-225348, V\-225347, V\-225346, V\-225345, V\-225344, V\-225341, V\-225340, V\-225339, V\-225338, V\-225337, V\-225329, V\-225326, V\-225325, V\-225323, V\-225322, V\-225321, V\-225320, V\-225317, V\-225316, V\-225315, V\-225314, V\-225305, V\-225304, V\-225303, V\-225302, V\-225301, V\-225300, V\-225299, V\-225298, V\-225297, V\-225296, V\-225295, V\-225294, V\-225293, V\-225292, V\-225291, V\-225290, V\-225289, V\-225288, V\-225287, V\-225286, V\-225285, V\-225284, V\-225283, V\-225282, V\-225281, V\-225280, V\-225279, V\-225278, V\-225277, V\-225276, V\-225275, V\-225273, V\-225272, V\-225271, V\-225270, V\-225269, V\-225268, V\-225267, V\-225266, V\-225265, V\-225264, V\-225263, V\-225261, V\-225260, V\-225259, and V\-225239
+ **Windows\\High**

  V\-225556, V\-225552, V\-225547, V\-225507, V\-225505, V\-225498, V\-225497, V\-225496, V\-225493, V\-225492, V\-225491, V\-225449, V\-225444, V\-225399, V\-225396, V\-225390, V\-225366, V\-225365, V\-225364, V\-225354, and V\-225274

## Microsoft \.NET Framework 4\.0 STIG V2 Release 1<a name="dotnet-os-stig"></a>

The following list contains STIG settings that are applied to Windows operating system components for STIG\-compliant Amazon EC2 AMIs\. Some STIG settings are not automatically applied\. This can be due to technical limitations – for instance, the STIG setting might not be applicable for standalone servers\. Organization\-specific policies can also prevent automatic application of STIG settings, such as a requirement for administrators to review document settings\. For more details about which STIGs are applied to Amazon EC2 Windows AMIs, you can download our [spreadsheet](https://aws-windows-downloads-us-west-1.s3.us-west-1.amazonaws.com/STIG/Win+STIG.xlsx)\.

For a complete list of Windows STIGs, see the [STIGs Document Library](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=windows)\. For information about how to view the complete list, see [SRG / STIG Tools](https://public.cyber.mil/stigs/srg-stig-tools/)\.
+ **Windows\\Low**

  No STIG settings are applied to the Microsoft \.NET Framework for Category III vulnerabilities\.
+ **Windows\\Medium**

  V\-225238
+ **Windows\\High**

  No additional STIG settings are applied for Category I vulnerabilities\.

## Windows Firewall STIG V1 Release 7<a name="windows-firewall-stig"></a>

The following list contains STIG settings that are applied to Windows operating system components for STIG\-compliant Amazon EC2 AMIs\. Some STIG settings are not automatically applied\. This can be due to technical limitations – for instance, the STIG setting might not be applicable for standalone servers\. Organization\-specific policies can also prevent automatic application of STIG settings, such as a requirement for administrators to review document settings\. For more details about which STIGs are applied to Amazon EC2 Windows AMIs, you can download our [spreadsheet](https://aws-windows-downloads-us-west-1.s3.us-west-1.amazonaws.com/STIG/Win+STIG.xlsx)\.

For a complete list of Windows STIGs, see the [STIGs Document Library](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=windows)\. For information about how to view the complete list, see [SRG / STIG Tools](https://public.cyber.mil/stigs/srg-stig-tools/)\.
+ **Windows\\Low**

  V\-17425, V\-17426, V\-17427, V\-17435, V\-17436, V\-17437, V\-17445, V\-17446, and V\-17447
+ **Windows\\Medium**

  V\-17415, V\-17416, V\-17417, V\-17419, V\-17429, and V\-17439
+ **Windows\\High**

  V\-17418, V\-17428, and V\-17438

## Internet Explorer \(IE\) 11 STIG V1 Release 19<a name="ie-os-stig"></a>

The following list contains STIG settings that are applied to Windows operating system components for STIG\-compliant Amazon EC2 AMIs\. Some STIG settings are not automatically applied\. This can be due to technical limitations – for instance, the STIG setting might not be applicable for standalone servers\. Organization\-specific policies can also prevent automatic application of STIG settings, such as a requirement for administrators to review document settings\. For more details about which STIGs are applied to Amazon EC2 Windows AMIs, you can download our [spreadsheet](https://aws-windows-downloads-us-west-1.s3.us-west-1.amazonaws.com/STIG/Win+STIG.xlsx)\.

For a complete list of Windows STIGs, see the [STIGs Document Library](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=windows)\. For information about how to view the complete list, see [SRG / STIG Tools](https://public.cyber.mil/stigs/srg-stig-tools/)\.
+ **Windows\\Low**

  V\-46477, V\-46629, and V\-97527
+ **Windows\\Medium**

  V\-46473, V\-46475, V\-46481, V\-46483, V\-46501, V\-46507, V\-46509, V\-46511, V\-46513, V\-46515, V\-46517, V\-46521, V\-46523, V\-46525, V\-46543, V\-46545, V\-46547, V\-46549, V\-46553, V\-46555, V\-46573, V\-46575, V\-46577, V\-46579, V\-46581, V\-46583, V\-46587, V\-46589, V\-46591, V\-46593, V\-46597, V\-46599, V\-46601, V\-46603, V\-46605, V\-46607, V\-46609, V\-46615, V\-46617, V\-46619, V\-46621, V\-46625, V\-46633, V\-46635, V\-46637, V\-46639, V\-46641, V\-46643, V\-46645, V\-46647, V\-46649, V\-46653, V\-46663, V\-46665, V\-46669, V\-46681, V\-46685, V\-46689, V\-46691, V\-46693, V\-46695, V\-46701, V\-46705, V\-46709, V\-46711, V\-46713, V\-46715, V\-46717, V\-46719, V\-46721, V\-46723, V\-46725, V\-46727, V\-46729, V\-46731, V\-46733, V\-46779, V\-46781, V\-46787, V\-46789, V\-46791, V\-46797, V\-46799, V\-46801, V\-46807, V\-46811, V\-46815, V\-46819, V\-46829, V\-46841, V\-46847, V\-46849, V\-46853, V\-46857, V\-46859, V\-46861, V\-46865, V\-46869, V\-46879, V\-46883, V\-46885, V\-46889, V\-46893, V\-46895, V\-46897, V\-46903, V\-46907, V\-46921, V\-46927, V\-46939, V\-46975, V\-46981, V\-46987, V\-46995, V\-46997, V\-46999, V\-47003, V\-47005, V\-47009, V\-64711, V\-64713, V\-64715, V\-64717, V\-64719, V\-64721, V\-64723, V\-64725, V\-64729, V\-72757, V\-72759, V\-72761, V\-72763, V\-75169, and V\-75171
+ **Windows\\High**

  No additional STIG settings are applied for Category I vulnerabilities\.

## Version history<a name="stig-version-history"></a>

The following table shows version history updates for STIG settings that are applied to Windows operating systems and Windows components\.


| Date | AMIs | Details | 
| --- | --- | --- | 
| 6/9/2021 |  Windows Server 2019 STIG V2 R2 Windows Server 2016 STIG V2 R2 Windows Server 2012 R2 STIG V3 R2 Microsoft \.NET Framework 4\.0 STIG V2 R1 Windows Firewall STIG V1 R7 Internet Explorer 11 STIG V1 R19  | Updated versions where applicable, and applied STIGs\. | 
| 4/5/2021 |  Windows Server 2019 STIG V2 R 1 Windows Server 2016 STIG V2 R 1 Windows Server 2012 R2 STIG V3 R 1 Microsoft \.NET Framework 4\.0 STIG V2 R 1 Windows Firewall STIG V1 R 7 Internet Explorer 11 STIG V1 R 19  | Updated versions where applicable, and applied STIGs\. | 
| 9/18/2020 |  Windows Server 2019 STIG V1 R 5 Windows Server 2016 STIG V1 R 12 Windows Server 2012 R2 STIG V2 R 19 Internet Explorer 11 STIG V1 R 19 Microsoft \.NET Framework 4\.0 STIG V1 R 9 Windows Firewall STIG V1 R 7  | Updated versions and applied STIGs\. | 
| 12/6/2019 | Server 2012 R2 Core and Base V2 R17 Server 2016 Core and Base V1 R11 Internet Explorer 11 V1 R18 Microsoft \.NET Framework 4\.0 V1 R9 Windows Firewall STIG V1 R17  | Updated versions and applied STIGs\. | 
| 9/17/2019 | Server 2012 R2 Core and Base V2 R16 Server 2016 Core and Base V1 R9 Server 2019 Core and Base V1 R2 Internet Explorer 11 V1 R17 Microsoft \.NET Framework 4\.0 V1 R8 | Initial release\. | 