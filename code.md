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
    
    ````