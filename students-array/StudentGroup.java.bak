package com.student;
import java.util.Date;
import java.util.Arrays;
import java.util.Calendar;

/**
 * A fix-sized array of students
 * array length should always be equal to the number of stored elements
 * after the element was removed the size of the array should be equal to the number of stored elements
 * after the element was added the size of the array should be equal to the number of stored elements
 * null elements are not allowed to be stored in the array
 * 
 * You may add new methods, fields to this class, but DO NOT RENAME any given class, interface or method
 * DO NOT PUT any classes into packages
 *
 */
public class StudentGroup implements StudentArrayOperation {

	private Student[] students;
	
	/**
	 * DO NOT remove or change this constructor, it will be used during task check
	 * @param length
	 */
	public StudentGroup(int length) {
		this.students = new Student[length];
	}

	@Override
	public Student[] getStudents() {
		// Add your implementation here
		for(int i=0;i<students.length;i++)
		{
			if(students[i]==null)
			{
				throw new IllegalArgumentException("there is no students to display");
			}
			else
			{
				System.out.println(students[i].getId());
                   System.out.println(students[i].getFullName());
				   System.out.println(students[i].getBirthDate());
				   System.out.println(students[i].getAvgMark());
			}
		return students;
	}

	@Override
	public void setStudents(Student[] students) {
		// Add your implementation here
		if(students==null)
		{
			throw new IllegalArgumentException(" students value is null");
		}
		else
		{
         for(int i=0;i<students.length;i++)
			{
			 add(students[i],i);
			}
		}
	}

	@Override
	public Student getStudent(int index) {
		// Add your implementation here
		if(students[index]==null)
		{
throw new IllegalArgumentException(" students value is null");
		}
		else
		{
System.out.println("getting values from index:"+index);
System.out.println(student[index].getId());
System.out.println(students[index].getFullName());
				   System.out.println(students[index].getBirthDate());
				   System.out.println(students[index].getAvgMark());
		}

		
		return students[index];
		}

	@Override
	public void setStudent(Student student, int index) {
		// Add your implementation here
		if(students==null)
		{
			throw new IllegalArgumentException(" students value is null");
		}
		else
		{
         
			 add(student,index);
		}
	}

	@Override
	public void addFirst(Student student) {
		// Add your implementation here
		if(student!=null)
		{
			add(student,0);
		}
		else
		{
throw new IllegalArgumentException(" students value is null");
		}

	}

	@Override
	public void addLast(Student student) {
		// Add your implementation here
		if(student!=null)
		{
			add(student,students.length-1);
		}
		else
		{
throw new IllegalArgumentException(" students value is null");
		}

	}

	@Override
	public void add(Student student, int index) {
		// Add your implementation here
		if(student!=null)
		{
			students[index]=student;
		}
		else
		{
throw new IllegalArgumentException(" students value is null");
		}
	}

	@Override
	public void remove(int index) {
		// Add your implementation here
		if(index < 0|| index >= students.length)
		{
throw new IllegalArgumentException(" students value is null");
		}
		else
		{
			for(int i=0;i<students.length;i++)
			{
				if(students[i]==students[index])
				{
					for(int j=i;j<students.length;j++)
					{
						students[j]=students[j+1];
					}
					break;
				}
			}
		}
	}

	@Override
	public void remove(Student student) {
		// Add your implementation here
		if(student==null)
		{
throw new IllegalArgumentException(" students value is null");
		}
		else
		{
			for(int i=0;i<students.length;i++)
			{
				if(students[i]==student)
				{
					remove(i);
					break;
				}
			}
		}

	}

	@Override
	public void removeFromIndex(int index) {
		// Add your implementation here

if(index < 0|| index >= students.length)
		{
throw new IllegalArgumentException(" students value is null");
		}
		else
		{
			remove(index);
		}

	}

	@Override
	public void removeFromElement(Student student) {
		// Add your implementation here
		if(student==null)
		{
throw new IllegalArgumentException(" students value is null");
		}
		else
		{
			for(int i=0;i<students.length;i++)
			{
				if(students[i]==student)
				{
					remove(i);
					break;
				}
			}
		}
	}

	@Override
	public void removeToIndex(int index) {
		// Add your implementation here
if(index < 0|| index >= students.length)
		{
throw new IllegalArgumentException(" students value is null");
		}
		else
		{
			for(int i=0;i<students.length;i++)
			{
				if(i!=index)
				{
					remove(index);
				}
			}
		}
	}

	@Override
	public void removeToElement(Student student) {
		// Add your implementation here
		if(student==null)
		{
throw new IllegalArgumentException(" students value is null");
		}
		else
		{
			for(int i=0;i<students.length;i++)
			{
				if(students[i]==student)
				{
					for(int j=0;j<i;j++)
					{
						remove(j);
					}
				}
			}
		}

	}

	@Override
	public void bubbleSort() {
		// Add your implementation here
for(int i=0;i<students.length;i++)
			{
	Student temp=null;
	if(students[i-1].getId() > students[i].getId())
				{
		temp=students[i-1];
students[i-1]=students[i];
students[i]=temp;
				}
			}
	}

	@Override
	public Student[] getByBirthDate(Date date) {
		// Add your implementation here
		if(students==null)
		{
			throw new IllegalArgumentException("no  students to display");
		}
		
		return null;
	}

	@Override
	public Student[] getBetweenBirthDates(Date firstDate, Date lastDate) {
		// Add your implementation here

		return null;
	}

	@Override
	public Student[] getNearBirthDate(Date date, int days) {
		// Add your implementation here
		return null;
	}

	@Override
	public int getCurrentAgeByDate(int indexOfStudent) {
		// Add your implementation here
		if(indexOfStudent<0||students.length<=indexOfStudent)
		{
			throw new IllegalArgumentException("no  students to display");
		}
		else
		{
			Calendar today=Calendar.getInstance();
			int todayYear=today.get(Calendar.YEAR);
			int birthDateYear=students[indexOfStudent].getBirthDate();
			int todayDayOfYear=today.get(Calendar.DAY_OF_YEAR);
			int birthDateDayOfYear=students[indexOfStudent].getBirthDate();
			int todayMonth=today.get(Calendar.MONTH);
			int birthDateMonth=students[i].getBirthDate();
			int todayDayOfMonth=today.get(Calendar.DAY_OF_MONTH);
			int birthDateDayOfMonth=students[i].getBirthDate();
			int totage=todayYear-birthDateYear;
			if((birthDateDayOfYear-todayDayOfYear>3)||(birthDateMonth>todayMonth))
			{
				totage--;
			}
			else if((birthDateMonth==todayMonth)&&(birthDateDayOfMonth>todayDayOfMonth))
			{
				totage--;
			}
			System.out.println("age is:"+totage);
		}
	}



		return students;
	}

	@Override
	public Student[] getStudentsByAge(int age) {
		// Add your implementation here
		


		return null;
	}

	@Override
	public Student[] getStudentsWithMaxAvgMark() {
		// Add your implementation here
		for(int i=0;i<students.length;i++)
		{
			if(students[i]==null)
			{
				throw new IllegalArgumentException("no  students to display");
			}
			else
			{
				System.out.println(students[i].getAvgMark());
			}
		}
		return null;
	}

	@Override
	public Student getNextStudent(Student student) {
		// Add your implementation here
		for(int i=0;i<students.length;i++)
		{
			if(student==null)
			{
				throw new IllegalArgumentException("no  students to display");
			}
			else
			{
				if(students[i]==student&&student[i]!=null)
				{
					System.out.println("next student details are:");
					System.out.println(students[i+1].getId());
					System.out.println(students[i+1].getFullName());
					System.out.println(students[i+1].getAvgMark());
				}
			}
		}


		return student;
	}
}
