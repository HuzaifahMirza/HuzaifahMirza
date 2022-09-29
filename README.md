

aboutMe 
--------------
Huzaifah Mirza,
male,
Montreal, Canada,
Skills: [java, html, css, javascript, python, kotlin (android development)]

public class readMe { 

	public static void main(String[] args) {
		aboutMe huzaifah = new aboutMe();
		String[] skills = {"java", "html", "css", "javascript", "python", "kotlin (android development)"};
		huzaifah.setSkills(skills);
		huzaifah.setLocation("Montreal, Canada");
		System.out.println(huzaifah.toString());

	}
	static class aboutMe {
		private final String name = "Huzaifah Mirza";
		private final String gender = "male";
		private String location;
		private String[] skills;

		public String getLocation() {
			return location;
		}

		public void setLocation(String location) {
			this.location = location;
		}

		public String[] getSkills() {
			return skills;
		}

		public void setSkills(String[] skills) {
			this.skills = skills;
		}

		public String getName() {
			return name;
		}

		public String getGender() {
			return gender;
		}

		@Override
		public String toString() {
			return "aboutMe " +"\n--------------" + "\n" + name + "\n" +gender +   "\n" + location + "\n"  + "Skills: " + Arrays.toString(skills);
		}

	}	

}

