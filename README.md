# Abstract_factory_methed


public abstract class Rbi_bank {
	public abstract void Rbi_bank();

}

public class Sbi_bank extends Rbi_bank {
	public void Rbi_bank() {
		System.out.println("rate interest");
		System.out.println("8 %");
	}
	

}

public class Sbi_factory {
	public static Rbi_bank getObj() {
		return new Sbi_bank();
	}
}


public class run_Rbi {
	public static void main(String[]args) {
		Rbi_bank r=Sbi_factory.getObj();
		r.Rbi_bank();  
		
		
	}

}
