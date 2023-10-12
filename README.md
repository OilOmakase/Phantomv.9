bounds_14 = getContentDescriptionByIdAndIndex("", 14);
bounds_15 = getContentDescriptionByIdAndIndex("", 15);
if(bounds_14 == null){notify14 ="กำลังทำงาน"}
else if(bounds_14 != null){
 kilo_14 = findAll(bounds_14, '.*[0-9].[0-9][[0-9][ ]].*');
 price_14 = findAll(bounds_14, '.*[0-9][0-9].[0-9].*');
 kilo_14_r1=replace(kilo_14, '[', '');
 kilo_14_r2=replace(kilo_14_r1, ']', '');
 kilo_14_fr = kilo_14_r2 ;
 price_14_r1=replace(price_14, '[', '');
 price_14_r2=replace(price_14_r1, ']', '');
 price_14_fr = price_14_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_14_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_16 = getContentDescriptionByIdAndIndex("", 16);
bounds_17 = getContentDescriptionByIdAndIndex("", 17);
if(bounds_16 == null){notify ="กำลังทำงาน"}
else if(bounds_16 != null){
 kilo_16 = findAll(bounds_16, '.*[0-9].[0-9][[0-9][ ]].*');
 price_16 = findAll(bounds_16, '.*[0-9][0-9].[0-9].*');
 kilo_16_r1=replace(kilo_16, '[', '');
 kilo_16_r2=replace(kilo_16_r1, ']', '');
 kilo_16_fr = kilo_16_r2 ;
 price_16_r1=replace(price_16, '[', '');
 price_16_r2=replace(price_16_r1, ']', '');
 price_16_fr = price_16_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_16_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_16_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_16_fr <= price_max and 
            price_16_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify16 = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_16_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_16_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_16_fr <= kilo_max and
                      kilo_16_fr >= kilo_min)
                      {
if(bounds_17 == "รับงาน"){
clickByIdAndIndex("", 17);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_14_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_16 = getContentDescriptionByIdAndIndex("", 16);
bounds_17 = getContentDescriptionByIdAndIndex("", 17);
if(bounds_16 == null){notify ="กำลังทำงาน"}
else if(bounds_16 != null){
 kilo_16 = findAll(bounds_16, '.*[0-9].[0-9][[0-9][ ]].*');
 price_16 = findAll(bounds_16, '.*[0-9][0-9].[0-9].*');
 kilo_16_r1=replace(kilo_16, '[', '');
 kilo_16_r2=replace(kilo_16_r1, ']', '');
 kilo_16_fr = kilo_16_r2 ;
 price_16_r1=replace(price_16, '[', '');
 price_16_r2=replace(price_16_r1, ']', '');
 price_16_fr = price_16_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_16_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_16_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_16_fr <= price_max and 
            price_16_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify16 = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_16_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_16_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_16_fr <= kilo_max and
                      kilo_16_fr >= kilo_min)
                      {
if(bounds_17 == "รับงาน"){
clickByIdAndIndex("", 17);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_14_fr <= price_max and 
            price_14_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_14_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_16 = getContentDescriptionByIdAndIndex("", 16);
bounds_17 = getContentDescriptionByIdAndIndex("", 17);
if(bounds_16 == null){notify ="กำลังทำงาน"}
else if(bounds_16 != null){
 kilo_16 = findAll(bounds_16, '.*[0-9].[0-9][[0-9][ ]].*');
 price_16 = findAll(bounds_16, '.*[0-9][0-9].[0-9].*');
 kilo_16_r1=replace(kilo_16, '[', '');
 kilo_16_r2=replace(kilo_16_r1, ']', '');
 kilo_16_fr = kilo_16_r2 ;
 price_16_r1=replace(price_16, '[', '');
 price_16_r2=replace(price_16_r1, ']', '');
 price_16_fr = price_16_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_16_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_16_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_16_fr <= price_max and 
            price_16_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify16 = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_16_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_16_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_16_fr <= kilo_max and
                      kilo_16_fr >= kilo_min)
                      {
if(bounds_17 == "รับงาน"){
clickByIdAndIndex("", 17);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_14_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_16 = getContentDescriptionByIdAndIndex("", 16);
bounds_17 = getContentDescriptionByIdAndIndex("", 17);
if(bounds_16 == null){notify ="กำลังทำงาน"}
else if(bounds_16 != null){
 kilo_16 = findAll(bounds_16, '.*[0-9].[0-9][[0-9][ ]].*');
 price_16 = findAll(bounds_16, '.*[0-9][0-9].[0-9].*');
 kilo_16_r1=replace(kilo_16, '[', '');
 kilo_16_r2=replace(kilo_16_r1, ']', '');
 kilo_16_fr = kilo_16_r2 ;
 price_16_r1=replace(price_16, '[', '');
 price_16_r2=replace(price_16_r1, ']', '');
 price_16_fr = price_16_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_16_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_16_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_16_fr <= price_max and 
            price_16_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify16 = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_16_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_16_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_18 = getContentDescriptionByIdAndIndex("", 18);
bounds_19 = getContentDescriptionByIdAndIndex("", 19);
if(bounds_18 == null){notify ="กำลังทำงาน"}
else if(bounds_18 != null){
 kilo_18 = findAll(bounds_18, '.*[0-9].[0-9][[0-9][ ]].*');
 price_18 = findAll(bounds_18, '.*[0-9][0-9].[0-9].*');
 kilo_18_r1=replace(kilo_18, '[', '');
 kilo_18_r2=replace(kilo_18_r1, ']', '');
 kilo_18_fr = kilo_18_r2 ;
 price_18_r1=replace(price_18, '[', '');
 price_18_r2=replace(price_18_r1, ']', '');
 price_18_fr = price_18_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_18_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
         else if(price_18_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
         else if(price_18_fr <= price_max and 
            price_18_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_18_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}}
              else if(kilo_18_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด";
bounds_20 = getContentDescriptionByIdAndIndex("", 20);
bounds_21 = getContentDescriptionByIdAndIndex("", 21);
if(bounds_20 == null){notify ="กำลังทำงาน"}
else if(bounds_20 != null){
 kilo_20 = findAll(bounds_20, '.*[0-9].[0-9][[0-9][ ]].*');
 price_20 = findAll(bounds_20, '.*[0-9][0-9].[0-9].*');
 kilo_20_r1=replace(kilo_20, '[', '');
 kilo_20_r2=replace(kilo_20_r1, ']', '');
 kilo_20_fr = kilo_20_r2 ;
 price_20_r1=replace(price_20, '[', '');
 price_20_r2=replace(price_20_r1, ']', '');
 price_20_fr = price_20_r2 ;
 if(price_max == null or price_min == null)
   {notify = "โปรดกำหนด'ราคา'"}
 else if(price_max < price_min)
        {notify = "'ราคา'ผิดพลาด"}
 else if(price_max >= price_min)
        {if(price_20_fr > price_max)
           {notify = "'ราคา'เกินกว่ากำหนด"}
         else if(price_20_fr < price_min)
                {notify = "'ราคา'ต่ำกว่ากำหนด"} 
         else if(price_20_fr <= price_max and 
            price_20_fr >= price_min)
           {if(kilo_max == null or 
               kilo_min == null){notify = "โปรดตั้งเงื่อนไขกิโล"}
             else if(kilo_max < kilo_min){notify = "'ระยะกิโล'ผิดพลาด"}
             else if(kilo_max >= kilo_min)
             {if(kilo_20_fr > kilo_max)
                {notify = "'ระยะกิโล'เกินกว่ากำหนด"}
              else if(kilo_20_fr < kilo_min)
                     {notify = "'ระยะกิโล'ต่ำกว่ากำหนด"} 
              else if(kilo_20_fr <= kilo_max and
                      kilo_20_fr >= kilo_min)
                      {
if(bounds_21 == "รับงาน"){
clickByIdAndIndex("", 21);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_18_fr <= kilo_max and
                      kilo_18_fr >= kilo_min)
                      {
if(bounds_19 == "รับงาน"){
clickByIdAndIndex("", 19);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_16_fr <= kilo_max and
                      kilo_16_fr >= kilo_min)
                      {
if(bounds_17 == "รับงาน"){
clickByIdAndIndex("", 17);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}} 
              else if(kilo_14_fr <= kilo_max and
                      kilo_14_fr >= kilo_min)
                      {
if(bounds_15 == "รับงาน"){
clickByIdAndIndex("", 15);
sleep(PHANToM_Delay);
PHANToM_CT = 1;
while(PHANToM_CT <= PHANToM_Round){
Num = 0;
PHANToM_List = [0 to 99];
shuffleList(PHANToM_List);
while(Num <= 99){
PHANToM_Element = getElement(PHANToM_List, Num);
if (PHANToM_Element <= 9){PHANToM = "0{PHANToM_Element}"}
else if (PHANToM_Element >= 10){PHANToM = "{PHANToM_Element}"};
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Notification = "เปลี่ยนคีย์บอร์ดด้วยจ้า";
sendText(PHANToM);
setSelection(0, 2);
sleep(PHANToM_Sleep);
 PHANToM_Sleep = (PHANToM_Sleep * PHANToM_Scale);
Num = (Num + 1);}
PHANToM_CT = PHANToM_CT + 1}
PHANToM = random(0,2);
}}}}}}
