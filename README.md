# ICF
package org.btm.setterinjectionApp;

public class AudiImpl implements ICar {
	
	  public AudiImpl() {
		System.out.println("Audi Implemantation Object Created");
	}
	
	
	@Overridepackage org.btm.setterinjectionApp;

import java.util.List;

public class BmwImpl implements ICar {
	
	private int id;
	private String color;
	private Engine engine;
	private List<String>wheels;
	public int getId() {
		return id;
	}
	public void setId(int id) {
		this.id = id;
	}
	public String getColor() {
		return color;
	}
	public void setColor(String color) {
		this.color = color;
	}
	public Engine getEngine() {
		return engine;
	}
	public void setEngine(Engine engine) {
		this.engine = engine;
	}
	public List<String> getWheels() {
		return wheels;
	}
	public void setWheels(List<String> wheels) {
		this.wheels = wheels;
	}
	@Override
	public void drive() {
		System.out.println("Bmw Car Deatils");
		System.out.println("Bmw Id "+getId());
		System.out.println("Bmw Color"+getColor());
		System.out.println("Bmw Engine"+getEngine());
		System.out.println("Bmw Wheels"+getWheels() );
		
	}
	 

}
package org.btm.setterinjectionApp;
public class Engine {

	private int engine_number;
	private int horse_power;
	private String type;
	public int getEngine_number() {
		return engine_number;
	}
	public void setEngine_number(int engine_number) {
		this.engine_number = engine_number;
	}
	public int getHorse_power() {
		return horse_power;
	}
	public void setHorse_power(int horse_power) {
		this.horse_power = horse_power;
	}
	public String getType() {
		return type;
	}
	public void setType(String type) {
		this.type = type;
	}
	  @Override
	public String toString() {
		
		  return "[Engine_number=" +engine_number+", Horse_Power=" +horse_power+", Type=" +type+"]";
	}
}
package org.btm.setterinjectionApp;
public interface ICar {

	void drive();
}
package org.btm.setterinjectionApp;

import org.springframework.context.ApplicationContext;
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class Test {

	
	public static void main(String[] args) {
		ApplicationContext ctx=new ClassPathXmlApplicationContext("Spring.xml");
		ICar i1=(ICar) ctx.getBean("bm");
		i1.drive();
		ICar i2=(ICar) ctx.getBean("ad");
		i2.drive();
	}
}

	public void drive() {
		System.out.println("Driving Audi Car Happily!!!!");
		
	}

}
package org.btm.setterinjectionApp;

import java.util.List;

public class BmwImpl implements ICar {
	
	private int id;
	private String color;
	private Engine engine;
	private List<String>wheels;
	public int getId() {
		return id;
	}
	public void setId(int id) {
		this.id = id;
	}
	public String getColor() {
		return color;
	}
	public void setColor(String color) {
		this.color = color;
	}
	public Engine getEngine() {
		return engine;
	}
	public void setEngine(Engine engine) {
		this.engine = engine;
	}
	public List<String> getWheels() {
		return wheels;
	}
	public void setWheels(List<String> wheels) {
		this.wheels = wheels;
	}
	@Override
	public void drive() {
		System.out.println("Bmw Car Deatils");
		System.out.println("Bmw Id "+getId());
		System.out.println("Bmw Color"+getColor());
		System.out.println("Bmw Engine"+getEngine());
		System.out.println("Bmw Wheels"+getWheels() );
		
	}
	 

}
package org.btm.setterinjectionApp;
public class Engine {

	private int engine_number;
	private int horse_power;
	private String type;
	public int getEngine_number() {
		return engine_number;
	}
	public void setEngine_number(int engine_number) {
		this.engine_number = engine_number;
	}
	public int getHorse_power() {
		return horse_power;
	}
	public void setHorse_power(int horse_power) {
		this.horse_power = horse_power;
	}
	public String getType() {
		return type;
	}
	public void setType(String type) {
		this.type = type;
	}
	  @Override
	public String toString() {
		
		  return "[Engine_number=" +engine_number+", Horse_Power=" +horse_power+", Type=" +type+"]";
	}
}
package org.btm.setterinjectionApp;
public interface ICar {

	void drive();
}
package org.btm.setterinjectionApp;

import org.springframework.context.ApplicationContext;
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class Test {

	
	public static void main(String[] args) {
		ApplicationContext ctx=new ClassPathXmlApplicationContext("Spring.xml");
		ICar i1=(ICar) ctx.getBean("bm");
		i1.drive();
		ICar i2=(ICar) ctx.getBean("ad");
		i2.drive();
	}
}
