class Toram {
    public String weapons;
    public String difficulity;
    public String optional;
    public Toram(String weapons, String difficulity, String optional) {
        this.weapons = weapons;
        this.difficulity = difficulity;
        this.optional = optional;
    }
}

public class Posttest1 {
    public static void main(String[] args) {
        Toram[] choose = new Toram[6];
        choose[0] = new Toram("1-H Sword", " (Easy)", "2-H Sword");
        choose[1] = new Toram("Staff", " (Hard)", "Magic Glider");
        choose[2] = new Toram("Knuckle", " (Easy)", "Enchance Knuckle");
        choose[3] = new Toram("Bow", " (Normal)", "Bowgun");
        choose[4] = new Toram("Halberd", " (Hard)", "+add pocket knife");
        choose[5] = new Toram("Katana", " (Normal)", "Enchance Katana");
        
        for (int i = 0; i < choose.length; i++) {
            System.out.print("\n Weapon " + (i + 1) + " : " + choose[i].weapons);
            System.out.print(choose[i].difficulity);
            System.out.print(" | Tier 2 : " + choose[i].optional);
            
        }
    }
}
