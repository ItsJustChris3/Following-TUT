using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

using Engine;
namespace firstgame
{
    public partial class firstgame : Form
    {
        private Player _player;

        public firstgame()
        {
            InitializeComponent();

            _player = new Player();

            _player.CurrentHitPoints = 10;
            _player.MaximumHitPoints = 10;
            _player.Gold = 40;
            _player.ExperiencePoints = 0;
            _player.Level = 1;
            
            lblHitPoints.Text = _player.CurrentHitPoints.ToString();
            lblGold.Text = _player.Gold.ToString();
            lblExperience.Text = _player.ExperiencePoints.ToString();
            lblLevel.Text = _player.Level.ToString();
        }
        private void label1_Click(object sender, EventArgs e)
        {

        }

    }     
        }
    

