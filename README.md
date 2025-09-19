# Corejava
package com.practiceex;

public class Stringlongestsequence{
	public static  String longestsequence (String s) {
  
	if(s == null || s.length()==0) return "";
	String current=" ";
		String longest=" ";
		
		for(int i=0; i<s.length(); i++) {
		if(current.length()==0|| s.charAt(i)>current.charAt(current.length()-1) ) {
			
	current +=s.charAt(i);
	if(current.length()>longest.length()) {
		longest=current;
	}
	
	}
		else {
			current= ""+s.charAt(i);
	
		}
	
		}
		return longest;
	}
	public static void main(String[]argu ) {
		String input="Crab";
		System.out.println("LongestSequence "+longestsequence(null));
	}
}


