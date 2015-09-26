# Classes
//By michael Revilla
// creates a random number between 1 and 6
// prints out the die number 
public class Classes {
	public static int die;

	public Classes() {
		die = 1;
	}

	public static void main(String[] args) {
		createPairOfDice();
		createPairOfDice();
	}

	public static void createPairOfDice() {
		die = getDieNum();
		printDie(die);
	}

	public static void printDie(int die) {
		if (die == 1) {
			System.out.println("-----------------");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "\t" + "*" + "\t" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("-----------------");
		} else if (die == 2) {
			System.out.println("-----------------");
			System.out.println("|" + "*" + "\t" + "\t" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "\t" + "       " + "*" + "|");
			System.out.println("-----------------");
		} else if (die == 3) {
			System.out.println("-----------------");
			System.out.println("|" + "\t" + "       " + "*" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "\t" + "*" + "\t" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "*" + "\t" + "\t" + "|");
			System.out.println("-----------------");
		} else if (die == 4) {
			System.out.println("-----------------");
			System.out.println("|" + "*" + "\t" + "       " + "*" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "*" + "\t" + "       " + "*" + "|");
			System.out.println("-----------------");
		} else if (die == 5) {
			System.out.println("-----------------");
			System.out.println("|" + "*" + "\t" + "       " + "*" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "\t" + "*" + "\t" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "*" + "\t" + "       " + "*" + "|");
			System.out.println("-----------------");
		} else {
			System.out.println("-----------------");
			System.out.println("|" + "*" + "\t" + "       " + "*" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "*" + "\t" + "       " + "*" + "|");
			System.out.println("|" + "\t" + "\t" + "|");
			System.out.println("|" + "*" + "\t" + "       " + "*" + "|");
			System.out.println("-----------------");
		}
	}

	public static int getDieNum() {
		int x;
		x = (int) (Math.random() * 6 + 1);
		return x;
	}
}
