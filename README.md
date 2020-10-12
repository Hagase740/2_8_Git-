# 2_8_Git-calculator2._0
class add_1 : Operator
    {
        public override void calcu(string x, string y)
        {
            Console.WriteLine("两字符串相加",x+y) ;
        }
    }
class reduce_1 : Operator
    {
        public override void calcu(string a, string b)
        {
            bool h = a.Contains(b);
            string c;
            if (h)
            {
                int i = a.IndexOf(b);
                c = a.Remove(i, b.Length);
                if (!c.Contains(b))
                {
                    Console.WriteLine("两字符串相减", c);
                }
                else
                    Console.WriteLine("无法进行减法");
            }
            else
                    Console.WriteLine("无法进行减法"); 
        }
    }
