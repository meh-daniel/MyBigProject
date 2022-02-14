static private string codeSms = "";
		public static void GenerateSms()
		{
			char[] letters = "QWERTYUIOPASDFGHJKL;Z'XCVBNM,.qwertyuiop[]asdfghjkl;'zcxvbnm,./123456788900-=`~*-+".ToCharArray();
			Random rand = new Random();
			string word = "";
			for (int i = 0; i < 9; i++) {
				int letter_num = rand.Next(0, letters.Length - 1);
				word += letters[letter_num];
			}
			codeSms = word;
		      codeSms.ToString();
		}
		public static string getSms()
		{
			return codeSms;
		}
