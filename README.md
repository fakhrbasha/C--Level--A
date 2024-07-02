# CSharp-Level--A
C# Level A

# Variable : 

(data type) (variable name) = Dec
 var -> فاريابول انت متعرفش هوا اي
int - float - char - bool - unit - long - ulong - double - string
-------------  ---------  ----------  ----------  ----
            int num;//var decleration
            num = 12; // var aggign
            Console.WriteLine(num);
            double num01 = 12.4;
            Console.WriteLine(num01);
            char num02= 'A';
            Console.WriteLine(num02);
            string num03 = ".NET";
            Console.WriteLine(num03);
            bool num04 = false; // true or false
            Console.WriteLine(num04);
            var num05 = "C# .NET";
            Console.WriteLine(num05);
            Console.WriteLine(int.MinValue) عشان اعرف data type دي بتشيل اقل رقم قد اي
             int x = 1;
            float y = 1.5f;// saffix
            decimal d = 10000m;
            Console.Write(default(int));
            
# Casting : 
           
            int x = 10;
            long y;
            y =x;
            float z = 1.32f;
            double d;
            d = z;
            // CONVERT 
            int k = Convert.ToInt32(d);
            Console.WriteLine(y);
            Console.WriteLine(k);
            Console.ReadLine(); 
            -------------------
# User Input : 
            Console.WriteLine("enter UR Name");
            // recive input from user (name)
                                                                                                                             // عرف فاريبول اديله اسم 
            string username=Console.ReadLine();
            // print user name
            Console.WriteLine("HI "+username);
            // age 
            Console.WriteLine("Enter UR Age ");
            int userage =Convert.ToInt32(Console.ReadLine());
                                                                                                   // لو معملتش convert  هيكون غي ايرور عشان هوا بيرجع string
            // print user age 
            Console.WriteLine("User Age : " + userage);
            --------------------

# Operation : 
            int a = 10;
            int b = 20;
            Console.WriteLine(a + b);// 30 
            string x = "C#";
            string y = ".NET";
            Console.WriteLine(x + y); // C#.NET
            double q = 10.0;
            double w = 5.0;
            Console.WriteLine(q /w); // 5.0
            // MOD
            Console.WriteLine(b%a); // 0
            ++q;
            Console.WriteLine(q); // 11
            bool e = q == w;
            Console.WriteLine(e); // false
            int t = 14;
            int u = 13;
            u += t;
            Console.WriteLine(u); // 27
            int f = sizeof(double);
            Console.WriteLine(f); // 8
            Type h = typeof(double);
            Console.WriteLine(h); // name datatype
            ----------------------
# Connditional statements :
 Console.WriteLine("if - else") ;
            int a = 10;
            int b = 20;
            if (a == b) // condition
            {
                Console.WriteLine(".NET");
            }
            else
            {
                Console.WriteLine("C#");
            }
            // output C#
            ---
 Console.WriteLine("if - else if - else") ;
            int a = 1;
            int b = 2;  
            if(a>b)
            {
                Console.WriteLine(".NET");
            }else if (a < b)
            {
                Console.WriteLine("C#");
            }
            else
            {
                Console.WriteLine("PY");
            }
            // output C#
            ---
   switch : 
    
            int b = Convert.ToInt32(Console.ReadLine());
            switch (b)
            {
                                                    // لو عايز 1 او 12 هينفذ نفس الشرط
                case 1:
                case 12:
                    Console.WriteLine("C#");
                    break;

                case 2:
                    Console.WriteLine(".NET");
                    break;

                default:                    default == else
                    Console.WriteLine("No Case");
                    break;
            }
    ---
             int a = 1;
                  int b = 2;
          int c;
          if(a > b){
              c = a + b;
          }
          else
          {
              c = a - b;
          }
           c = (a > b) ? (a + b) : (a - b);
          Console.WriteLine(c);
          // ternary operator ?:
         
          // expretion  ?true : false 
       ------------------------

# Loop : 
             int a = 0; // init
          
           while (a<5) // condition
           {
               Console.WriteLine(".NET");
               a++; // inc
           }
                                                                                           // لو عايز اعمل لوب مرة
           // do while 
           do
           {
               Console.WriteLine("C#");
           } while (a ==7);
           // for
           for(int i = 0; i < 5; i++)
           {
               Console.WriteLine("Fakhr Basha , " + i);
           }
                                                                                                                           
           // . break , continue
           // break  بتخرجك من اللوب برا خالص
           // continue  بتعمل skip لحاجة معينة
           for(int i = 0; i < 5; i++)
           {
               
               if(i== 3)
               {
                   break; 
               }
               Console.WriteLine(".Net , " +i );
           }
           Console.WriteLine("------continue------");
           for (int i = 0; i < 5; i++)
           {
          
               if (i == 3)
               {
                   continue;
               }
               Console.WriteLine(".Net , " + i);
           }
    ------------------------------
# Array : 

             int[] array01 = new int[6]; // كدا عرفت اراي ف الميموري وعددها 6 عناصر
            
             int[] array02 = new int[3] {4 , 5 , 7 }; // assignment 1
            
             int[] array03 = new int[] {4 , 5 , 7 }; // assignment 2
            
             int[] array04 = {4 , 5 , 7 }; // assignment  3
            
             int[] array05;
             array05 =new int[] {2,4,5,6}; // assignment  4
            
            
            string[] arr = new string[3] { "ahmed", "Mo", "Salah" };
            
            string name = arr[1];
            
            arr[0] = "Fakhr";
            
            Console.WriteLine(name);
            
            Console.WriteLine(arr[0]);
            
            Console.WriteLine(arr.Length);  // length array
            
            Console.WriteLine("-----------");
            
            // print element in array
            for (int i=0; i < arr.Length; i++)
            {
                Console.WriteLine(arr[i]);
            }
            Console.WriteLine("-----------");
            
            // for each
            arr[2] = "Basha";
            foreach (var y in arr)
            {
                Console.WriteLine(y);
            }
            Console.WriteLine("-----------");
            // min element
            int[] arrx = new int[] { 12, 4, 5, 7, 8 };
            Console.WriteLine( "Min Value : " +arrx.Min());
            Console.WriteLine("-----------");
            // max element 
            Console.WriteLine( "Max Value : " +arrx.Max());
            Console.WriteLine("-----------");
            // print sum of array
            Console.WriteLine("Sum : "+arrx.Sum());
            Console.WriteLine("-----------");
            // print avg 
            Console.WriteLine("Avarage : "+arrx.Average());
            Console.WriteLine("-----------");
            // sort 
            Array.Sort(arrx);
            Console.WriteLine(arrx[0])

-----------------------------------------

# Multi-dimensional & Jagged array : 

            int [] arr = new int[] {1,2,3}; // 1D
            Console.WriteLine(arr[0]);
            // 2D array dec

            int[,] twoD = new int[2, 3] { {1,2,3 }, {4,5,6 } }; // 2D
                                                                // 2 row  3 colum
            Console.WriteLine(twoD[1,1]); // 5
            Console.WriteLine(twoD[0,1]); // 2
            twoD[0,2] = 11;
            Console.WriteLine(twoD[0, 2]);
            Console.WriteLine("-----------"); 
            foreach (var item in twoD)
            {
                Console.WriteLine(item);
            }
            Console.WriteLine("-----------");
            // nested loop
            for (int i = 0; i < 2; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    Console.WriteLine(i + " " + j + " " + " -> " + twoD[i, j]);
                }
            }
            // Jagged aray ملهاش تكوين ثابت 
            int[][] jag = new int[3][] {
                new int[3]{ 1, 2, 3 },
                new int[2] { 5, 6 },
                new int [4] { 7, 8, 9, 10 } 
            }; 
---------------           --------------------- 
# String : 

            Console.WriteLine(".Net");

            string s1 = "Hello C#";
            // string array of char

            char[] arrstr = new char[] { '.', 'N', 'E', 'T' };

            string s2 = new string(arrstr);  // كدا كونت سترينج جديد 
            Console.WriteLine(arrstr);
            Console.WriteLine(arrstr[3]); // T

            Console.WriteLine("Length : " + arrstr.Length);
            // عايز اعرف مكان حرف معين 
            Console.WriteLine(s2.IndexOf('E')); // 2
            Console.WriteLine(" ------------- ");
              // اطبع من مكان معين 
            string s3 = "C# .Net";
            string m = s3.Substring(3); // هقطع اي حاجة قبل idx 3
            Console.WriteLine(m); // .Net
            string q = s3.Substring(s3.IndexOf('.'));
            Console.WriteLine(q);
            Console.WriteLine(" ------------- ");
            // compare
            string c1 = "Ahmed";
            string c2 = "Mohamed";
            int res = String.Compare(" c1 < c2 :  " + c1, c2);
            Console.WriteLine(res);
            // لو الاتنين مش زي بعض بالظبط هيطلع -1 لو زي بعض بيطلع 0
            string a1 = "Ahmed";
            string a2 = "Ahmed";
            int res2 = String.Compare("a1 = a2 : "+ a1, a2);
            Console.WriteLine(res2);
            // لو الاول اكبر من التاني هيطبع 1
            string b1 = "AhmedB";
            string b2 = "Ahmed";
            int res3 = String.Compare("b1 > b2 : " + b1, b2);   
            Console.WriteLine(res3);

            Console.WriteLine(" ------------- ");
            // عايز اعرف كلمة معينة موجودة ولا لا  contains
            string c01 = "C# .NET";
            if (c01.Contains("C#"))
            {
                Console.WriteLine("YES");
            }
            else
            {
                Console.WriteLine("NO");
            }
            Console.WriteLine(" ------------- ");
            // convert to upper case
            string c02 = "Fakhr Basha";
            Console.WriteLine(c02.ToUpper());
            Console.WriteLine(c02.ToLower());
            Console.WriteLine(" ------------- ");
            // special Character
            // "Hello "ahmed " "; skaping \ \

            string c03 = "Hello\"Ahmed\" ";
            Console.WriteLine(c03);

            // لو عايز اطبع كل اللي ف الاسترنج زي مهوا (@)

            string c04 = @"Hello \n .Net ";
            Console.WriteLine(c04);
            // لو شيلت @ هينزل سطر 
            Console.WriteLine(" ------------- ");
            // string concatenation
            string c05 = "C# ";
            string c06 = ".Net";
            Console.WriteLine(c05+c06);

            // other String concat
            Console.WriteLine(String.Concat(c05 + c06));
            // string interpolation $  " {variable} string " ;
            int x = 10;
            string s = "Salary";
            string res04 = $"{s} = {x}";
            Console.WriteLine(res04);   
-------------- -------------- -------------
# Constants & Nullables : 

runtime : 
    int [] array = new int [] {1,2,3} 
    Console.WriteLine(array[5]);  runtime err0r
compile time : 
    int x = 10            forget (;)

 

            int? x = null;
            Nullable<double> y = null; // value type
            string c = null; // ref type
                             // coalscing operator

            // int z;
            // z = x; // error becouse x NULL
            y = x ?? 14; // if x nut null y = 15 otherwise y = x
            Console.WriteLine(y);
--------- --------- ----------- ---------- 

# Exception Handling : 
ازاي تتعامل مع error


 //                 انا متوقع هما ممكن يحصل ايرور -> try catch
            try
            {
                int[] values = { 12, 13, 20 };
                Console.WriteLine(values[6]);

                int a = 10; 
                int b = 5;
                int res = a / b; // error
            }
            catch (IndexOutOfRangeException e)
            {
                // رسالة اعرفهه ان في ايرور 
                Console.WriteLine(e.Message); //الرسالة بتاع الايرور 
                Console.WriteLine("Error , Please Try Again\n"); 
                 // index out of range
                // تفكر ف الايرور وتعملها handleng
            }
            catch (DivideByZeroException c)
            {
                Console.WriteLine(c.Message);
                Console.WriteLine("Not allowed Divide By Zero\n");
            }
            finally
            {
                Console.WriteLine("Operation Done"); // كود بيتنفذ ف الاخر بعد مالكاتش تخلص
            }
            Console.WriteLine("----------");

            Console.WriteLine("Enter The First Num");

            string fnum = Console.ReadLine();

            Console.WriteLine("Enter Second Num");

            string snum= Console.ReadLine();
            try
            {
                int res=Convert.ToInt32(fnum)/Convert.ToInt32(snum);
                Console.WriteLine(res);

            }
            catch (Exception e) 
            {
                    Console.WriteLine(e.Message);
            }
            finally
            {
                
                Console.WriteLine("Operation Done");
            }
------------ ----------- ------------
# Methods: Function :


            int x = 10; int y= 20;

            int sum=x + y;

            int a = 20; int b = 30;

            int sum2=a+b;


            Console.WriteLine(sum);
            Console.WriteLine(sum2);

            // DRY don't repeat yourself

            addnum(x,y); // calling
            addnum(a,b);

            Console.WriteLine(div(y,x)); // Calling method 2

            name();

            Console
                .WriteLine("Enter Number : ");

            
            int s = Convert.ToInt32(Console.ReadLine());
            int l = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine(mx(l,s));


            string namee=Console.ReadLine();
            Console.WriteLine("Enter Name : ");
            Console.WriteLine(sayhi(namee));


-- out main function --
            // public : access modefier    || private
        // void : return type    (void || int || double .....)
        // addnum : method name 
        // (int x , int y) : parametar List
        public static void addnum(int x, int y) // method
        {
            Console.WriteLine(x + y);
        }


        public static int div(int z, int n)
        {
            return(z / n);
        }


        private static void name()
        {
            Console.WriteLine(".Net");
        }


        // get max
        private static int mx(int w, int r = 1) { // r defult number = 1 
            if (w > r)
            {
                return w;
            }
            else
            {
                return r;
            }
        }


        private static string sayhi(string name)
        {
            string result = $"Hi {name}";
            return result;
        }
----------- --------------- ------------- ------------
# passing parameters: 
* by value
* by refrance 
* by out
* by params

           
            
            int a = 10;
            int b = 20;
            // passing by value
            int res =addnum(a, b);
            Console.WriteLine(res); // 30
            Console.WriteLine(a); // مش هتتغير 


            Console.WriteLine("----------");
            // refrance
            int res2=adnum(ref a,ref b);
            Console.WriteLine(res2);
            Console.WriteLine(a); //11

            Console.WriteLine("----------");
            // out
            int res3;
            int res4;
            adddnum(a, b, out res3,out res4); // also passing by ref
            Console.WriteLine(res3);
            Console.WriteLine(res4);

            Console.WriteLine("----------");
            // params

            int sum = addnum4(2, 4, 7, 9);
            Console.WriteLine(sum);


            Console.WriteLine("----------"); // calling

            printname("Ahmed", "Mohamed", "Salah");
--- --- out main --- --- --


       // method sum
        public static int addnum(int x, int y = 1) { // defult y = 1

            int summ = x + y  ;

            x++; // مش هتتغير فوق

            return summ;

        }
        // passing by refrance
        public static int adnum(ref int x, ref int y )
        { 

            int summ = x + y;

            x++; //  هتتغير فوق

            return summ;

        }

        public static void adddnum( int x,  int y , out int sum , out int mult)
        { 

             sum = x + y;
            mult = x * y;
            x++; //  هتتغير فوق

            

        }

        public static int addnum4(params int[] number ) // لو عايز اجمع اراي paramms
        {

            int sum = 0;
            foreach (int num in number)
            {
                sum+= num;
            }

            return sum;

        }


        public static void printname(params string[] names)
        {
            foreach (string name in names)
            {
                Console.WriteLine(name);
            }

        }
----------------------------------------------
# Recursion & Overloading : 
Recursion : 
    
                    //factorial
            // 4! = 4 * 3 * 2 *1 == 24
            // m! = m * (m-1)
            // 0! = 1

            Console.WriteLine("Before Rec : " + factorial(4)); // 12

            Console.WriteLine("After Rec : " + factorial2(4)); 

------- out main Func -------
        // recursion function call itself
        // دي كدا دالة عادية هتضرب x * x-1 بس
    
           static int factorial(int x)
         { 

            int res = x * (x-1);

            return res;
        }

        static int factorial2(int x)

        {
            // base case اللي للازم تقف عندها
            if (x == 0) {
                return 1;
            }

            int res = x * factorial2(x - 1);

            return res;
        }

----------- Overloading ----------

            // overloading :  function use same name but deffirant prameter (signature)
            int y = addnumber(5, 10);

            double z = addnumber(5.2, 10.4);

            Console.WriteLine(y);

            Console.WriteLine(z);
 --- out main ----

          public static int addnumber(int x , int y)
        {
            int res= x+y;
            return res; 
        }

        public static double addnumber(double x, double y)
        {
            double res = x + y;
            return res;
        }
------------------------------------------------------
# Debugging : 
    مهارة اكتشاف الاخطاء وحلها من IDE
            int x = 50;
            int y = 30;

            // break point f9 لو عملت debug  هيقف عند اول break point
            // تتحرك ف الكود عن طريق f10

            int sum = x + y ;
            int sub = x - y;
            int multiply = x * y;
            int div = x / y;
            // لو عايز اراقب عنصر معين اعمله watch -> right click -> add watch
           Console.WriteLine(sum);

            Console.WriteLine("----------");

            int res = add(x, y);

            Console.WriteLine(res);

            Console.WriteLine("----------");
            int[] arr = { 1, 23, 4 };
            foreach (int i in arr)
            {
                Console.WriteLine(i);
            }
-- method --
         // debug method (f11) step into
        // exit from method  step out  (shift+f11)
        private static int add(int x, int y)
        {
            int sum = x + y;

            return sum;
        }
------------------------------ Console.WriteLine( "Hello, World " ); ------------------------- Fakhr Basha ----------------------------------------------






            
