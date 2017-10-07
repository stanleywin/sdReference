##

````c#
protected void Button1_Click(object sender, EventArgs e)
    {
        int[] n = new int[5];
        string s = "";
        for(int i = 1; i <= 5; i++)
        {
            n[i - 1] = i;
            s = s + n[i - 1].ToString() + " ";
        }
        Label1.Text =s;
    } 


protected void Button1_Click(object sender, EventArgs e)
    {
        int[] n = new int[5];
        var s = "";
        for(int r in n)
        { 
            s = s + r.ToString() + " ";
        }
        Label1.Text = s;
    }
    
    protected void Button1_Click(object sender, EventArgs e)
    {
        string r = "";
        List<int> mArray = new List<int>(); //List is a data structure (template) 
        mArray.Add(5);
        mArray.Add(10);
        mArray.Add(3);
        Label1.Text = mArray.Count.ToString();
        mArray.Sort(); // sort by the num sequence
        foreach (int num in mArray)
            r += num.ToString() + " ";
        Label2.Text = r;
    }

 protected void Button1_Click(object sender, EventArgs e)
    {
        string r = "";
        List<string> mArray = new List<string>();
        mArray.Add("banana");
        mArray.Add("apple");
        mArray.Add("cat");
        Label1.Text = mArray.Count.ToString();
        mArray.Sort(); //sort by a-z
        foreach (string num in mArray)
            r += "" + num.ToString() + " ";
        Label2.Text = r;
    }
    
 using System.Collections;
 
 protected void Button1_Click(object sender, EventArgs e)
    {
        string r = "";
        ArrayList mArray = new ArrayList();
        mArray.Add("banana");
        mArray.Add("apple");
        mArray.Add("cat");
        Label1.Text = mArray.Count.ToString();
        mArray.Sort();
        foreach (string num in mArray)
            r += "" + num.ToString() + " ";
        Label2.Text = r;
    }
    
        protected void Button1_Click(object sender, EventArgs e)
    {
        ArrayList mArray = new ArrayList();
        DateTime dt = DateTime.Now;
        for (int i = 1; i <= 1000000; i++)
            mArray.Add(i);
        TimeSpan ts = DateTime.Now - dt;
        Label1.Text = ts.Milliseconds + "ms";
        
    }
    
        protected void Button1_Click1(object sender, EventArgs e)
    {
        string r = TextBox1.Text;
        r = r.Replace("\r\n", "<br>");
        r = "<hr>" + DateTime.Now + "<br>" + TextBox2.Text + "<br>" + r;
        Label1.Text = r + Label1.Text;
    }
    
    ````