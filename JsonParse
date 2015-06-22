package br.com.studies.JsonParse;

import java.io.FileNotFoundException;
import java.io.FileReader;
import java.io.IOException;
import org.json.simple.JSONArray;
import org.json.simple.JSONObject;
import org.json.simple.parser.JSONParser;
import org.json.simple.parser.ParseException;

public class JsonParse {

	private static String jsonFile = "C:\\Users\\Fabio\\Desktop\\json.json";
	public static void main(String[] args) {
		try {		
			//Here, we will read the file
			FileReader reader;
	
				reader = new FileReader(jsonFile);
			
			//Here, we will use the library to read the Json file
			JSONObject jsonObject = (JSONObject) new JSONParser().parse(reader);
			
			//Taking the name
			String name = (String) jsonObject.get("name");
			System.out.println(name);
			
			JSONArray lang = (JSONArray) jsonObject.get("languages");
			
			for(int i=0; i<lang.size(); i++){
				System.out.println(lang.get(i)+ "\n");	
			}
		} catch (FileNotFoundException e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		} catch (IOException e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		} catch (ParseException e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		}
		
		
	}

}
