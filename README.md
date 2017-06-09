# JSONFiledAdd
将一个json数据的的某一个字段转换成拼音然后返回新的添加了拼音字段的json数据，也可以转换List&lt;Map>中指定key的value

![image](https://github.com/CustomViewDemo/findinitialsutils/Screenshot/master/json.png)

for (int i = 0; i < 10; i++) {
            Map<String, Object> map = new HashMap<>();
            map.put("name", "地方"+i);
            map.put("address","江西"+i);
            map.put("description","激发大家发垃圾分类");
            map.put("age",i);
            listMap.add(map);
        }
        
 new FindInitialsUtils("name").ListMapToJson(listMap);
 
 
 String str2 = "{ \"programmers\": [ { \"firstName\": \"Brett\", \"lastName\":\"McLaughlin\", \"email\": \"aaaa\" },\n" +
                "\n" +
                "{ \"firstName\": \"Jason\", \"lastName\":\"Hunter\", \"email\": \"bbbb\" },\n" +
                "\n" +
                "{ \"firstName\": \"Elliotte\", \"lastName\":\"Harold\", \"email\": \"cccc\" }\n" +
                "\n" +
                "],\n" +
                "\n" +
                "\"authors\": [\n" +
                "\n" +
                "{ \"firstName\": \"Isaac\", \"lastName\": \"Asimov\", \"genre\": \"science fiction\" },\n" +
                "\n" +
                "{ \"firstName\": \"Tad\", \"lastName\": \"Williams\", \"genre\": \"fantasy\" },\n" +
                "\n" +
                "{ \"firstName\": \"Frank\", \"lastName\": \"Peretti\", \"genre\": \"christian fiction\" }\n" +
                "\n" +
                "],\n" +
                "\n" +
                "\"musicians\": [\n" +
                "\n" +
                "{ \"firstName\": \"Eric\", \"lastName\": \"Clapton\", \"instrument\": \"guitar\" },\n" +
                "\n" +
                "{ \"firstName\": \"Sergei\", \"lastName\": \"Rachmaninoff\", \"instrument\": \"piano\" }\n" +
                "\n" +
                "] }";
                               
 new FindInitialsUtils("firstName").AddPinyinfieldToJson(str2)
