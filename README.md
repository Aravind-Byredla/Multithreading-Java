# Multithreading-Java


import java.io.*;

class Test extends Thread{
    public void run(){
        for (int i=0; i<5; i++){
            System.out.println("Test Thread");
        } 
    }
}

class GFG {
	public static void main (String[] args) {
		Test t = new Test();
		t.start();
		for (int i=0; i<5; i++){
		    System.out.println("Main Thread");
		} 
	}
}
