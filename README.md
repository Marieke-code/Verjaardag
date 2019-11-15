# Verjaardag
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Verjaardag
{
          class Scherm : Form
        {
            private TextBox Dag;
            private TextBox Maand;
            private TextBox Jaar;
            private Label Leeftijd;

            public Scherm()
            {
                Label tekst;
                Button knop;

                tekst = new Label();
                knop = new Button();
                this.Dag = new TextBox();
                this.Maand = new TextBox();
                this.Jaar = new TextBox();
                this.Leeftijd = new Label();

                tekst.Location = new Point(0, 0);
                knop.Location = new Point(0, 150);
                this.Dag.Location = new Point(110, 6);
                this.Maand.Location = new Point(110, 6);
                this.Jaar.Location = new Point(110, 6);
                this.Leeftijd.Location = new Point(110, 34);
                tekst.Size = new Size(35, 20);
                knop.Size = new Size(80, 20);
                this.Dag.Size = new Size(80, 20);
                this.Maand.Size = new Size(80, 20);
                this.Jaar.Size = new Size(80, 20);
                this.Leeftijd.Size = new Size(120, 20);
                tekst.Text = "geboortedatum";
                knop.Text = "leeftijd";
                knop.Click += this.bereken;
                
        }

    }
}
