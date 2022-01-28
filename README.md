# sushma.
#TicTacToe
import java.awt.EventQueue;

import javax.swing.JFrame;
import javax.swing.JPanel;
import javax.swing.border.LineBorder;
import java.awt.Color;
import java.awt.GridLayout;
import javax.swing.JLabel;
import javax.swing.JOptionPane;
import javax.swing.JButton;
import java.awt.event.ActionListener;
import java.awt.event.ActionEvent;
import java.awt.Font;
import javax.swing.SwingConstants;
import javax.swing.JTextField;

public class TicTacToe {

	private JFrame frame;
	private JTextField xCount;
	private JTextField oCount;
	private int xCount1=0;
	private int oCount1=0;
	private String startGame = "X";
	private int b1=10;
	private int b2=10;
	private int b3=10;
	private int b4=10;
	private int b5=10;
	private int b6=10;
	private int b7=10;
	private int b8=10;
	private int b9=10;
	private int i=0;

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					TicTacToe window = new TicTacToe();
					window.frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the application.
	 */
	public TicTacToe() {
		initialize();
	}
	
	private void winningGame()
	//FOR PLAYER X ALONE THE NUMBER OF POSSIBLE WINNING CHANCES ARE MENTIONED
	{
		if(b1==1 && b2==1 && b3==1)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER X WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			xCount1++;
			xCount.setText(String.valueOf(xCount1));
		}
		else if(b4==1 && b5==1 && b6==1)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER X WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			xCount1++;
			xCount.setText(String.valueOf(xCount1));
		}
		else if(b7==1 && b8==1 && b9==1)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER X WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			xCount1++;
			xCount.setText(String.valueOf(xCount1));
		}
		else if(b1==1 && b4==1 && b7==1)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER X WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			xCount1++;
			xCount.setText(String.valueOf(xCount1));
		}
		else if(b2==1 && b5==1 && b8==1)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER X WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			xCount1++;
			xCount.setText(String.valueOf(xCount1));
		}
		else if(b3==1 && b6==1 && b9==1)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER X WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			xCount1++;
			xCount.setText(String.valueOf(xCount1));
		}
		else if(b1==1 && b5==1 && b9==1)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER X WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			xCount1++;
			xCount.setText(String.valueOf(xCount1));
		}
		else if(b3==1 && b5==1 && b7==1)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER X WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			xCount1++;
			xCount.setText(String.valueOf(xCount1));
		}
		
		
		//FOR PLAYER O ALONE THE NUMBER OF POSSIBLE WINNING CHANCES ARE MENTIONED
	
	   	
		else if(b1==0 && b2==0 && b3==0)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER O WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			oCount1++;
			oCount.setText(String.valueOf(oCount1));
		}
		else if(b4==0 && b5==0 && b6==0)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER O WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			oCount1++;
			oCount.setText(String.valueOf(oCount1));
		}
		else if(b7==0 && b8==0 && b9==0)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER O WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			oCount1++;
			oCount.setText(String.valueOf(oCount1));
		}
		else if(b1==0 && b4==0 && b7==0)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER O WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			oCount1++;
			oCount.setText(String.valueOf(oCount1));
		}
		else if(b2==0 && b5==0 && b8==0)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER O WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			oCount1++;
			oCount.setText(String.valueOf(oCount1));
		}
		else if(b3==0 && b6==0 && b9==0)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER O WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			oCount1++;
			oCount.setText(String.valueOf(oCount1));
		}
		else if(b1==0 && b5==0 && b9==0)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER O WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			oCount1++;
			oCount.setText(String.valueOf(oCount1));
		}
		else if(b3==0 && b5==0 && b7==0)
		{
			JOptionPane.showMessageDialog(frame,"GREAT!!! PLAYER O WINS THE GAME","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			oCount1++;
			oCount.setText(String.valueOf(oCount1));
		}
		else if(i==9)
		{
			JOptionPane.showMessageDialog(frame,"IT'S A TIE, THINK OF A TIEBREAKER , PLAY AGAIN","Tic Tac Toe",JOptionPane.INFORMATION_MESSAGE);
			
		}}
	
	
	private void choosePlayer()
	{
		if(startGame.equalsIgnoreCase("X"))
		{
			startGame = "O";
		}
		else 
		{
			startGame = "X";
		}
	}

	/**
	 * Initialize the contents of the frame.
	 */
	private void initialize() {
		frame = new JFrame();
		frame.setBounds(100, 100, 1200, 1200);
		frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		frame.getContentPane().setLayout(null);
		
		JPanel panel = new JPanel();
		panel.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.setBounds(0, 0, 776, 563);
		frame.getContentPane().add(panel);
		panel.setLayout(new GridLayout(3, 5, 2, 2));
		
		JPanel panel_1 = new JPanel();
		panel_1.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_1);
		
		JButton btn1 = new JButton("");
		btn1.setBackground(Color.PINK);
		btn1.setFont(new Font("Tahoma", Font.BOLD, 80));
		btn1.setBounds(10, 10, 132, 164);
		btn1.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				btn1.setText(startGame);
				if(startGame.equalsIgnoreCase("X"))
				{
					btn1.setForeground(Color.red);
					b1=1;
					i++;
				}
				else
				{
					btn1.setForeground(Color.blue);
					b1=0;
					i++;
				}
				choosePlayer();
				winningGame();
			}
		});
		panel_1.setLayout(null);
		panel_1.add(btn1);
		
		JPanel panel_2 = new JPanel();
		panel_2.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_2);
		panel_2.setLayout(null);
		
		JButton btn2 = new JButton("");
		btn2.setBackground(Color.PINK);
		btn2.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				btn2.setText(startGame);
				if(startGame.equalsIgnoreCase("X"))
				{
					btn2.setForeground(Color.red);
					b2=1;
					i++;
				}
				else
				{
					btn2.setForeground(Color.blue);
					b2=0;
					i++;
				}
				choosePlayer();
				winningGame();
			}
		});
		btn2.setFont(new Font("Tahoma", Font.BOLD, 80));
		btn2.setBounds(10, 10, 132, 164);
		panel_2.add(btn2);
		
		JPanel panel_3 = new JPanel();
		panel_3.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_3);
		
		JButton btn3 = new JButton("");
		btn3.setBackground(Color.PINK);
		btn3.setFont(new Font("Tahoma", Font.BOLD, 80));
		btn3.setBounds(10, 10, 132, 164);
		btn3.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				btn3.setText(startGame);
				if(startGame.equalsIgnoreCase("X"))
				{
					btn3.setForeground(Color.red);
					b3=1;
					i++;
				}
				else
				{
					btn3.setForeground(Color.blue);
					b3=0;
					i++;
				}
				choosePlayer();
				winningGame();
			}
		});
		panel_3.setLayout(null);
		panel_3.add(btn3);
		
		JPanel panel_4 = new JPanel();
		panel_4.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_4);
		panel_4.setLayout(null);
		
		JLabel lblNewLabel = new JLabel("  PLAYER X");
		lblNewLabel.setBackground(new Color(0, 0, 0));
		lblNewLabel.setForeground(Color.MAGENTA);
		lblNewLabel.setFont(new Font("Microsoft New Tai Lue", Font.BOLD, 25));
		lblNewLabel.setBounds(10, 10, 132, 164);
		panel_4.add(lblNewLabel);
		
		JPanel panel_5 = new JPanel();
		panel_5.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_5);
		panel_5.setLayout(null);
		
		xCount = new JTextField();
		xCount.setHorizontalAlignment(SwingConstants.CENTER);
		xCount.setBackground(Color.YELLOW);
		xCount.setForeground(Color.RED);
		xCount.setFont(new Font("Tw Cen MT Condensed Extra Bold", Font.BOLD, 45));
		xCount.setText("     0");
		xCount.setBounds(10, 10, 132, 164);
		panel_5.add(xCount);
		xCount.setColumns(10);
		
		JPanel panel_6 = new JPanel();
		panel_6.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_6);
		panel_6.setLayout(null);
		
		JButton btn4 = new JButton("");
		btn4.setBackground(Color.PINK);
		btn4.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				btn4.setText(startGame);
				if(startGame.equalsIgnoreCase("X"))
				{
					btn4.setForeground(Color.red);
					b4=1;
					i++;
				}
				else
				{
					btn4.setForeground(Color.blue);
					b4=0;
					i++;
				}
				choosePlayer();
				winningGame();
			}
		});
		btn4.setFont(new Font("Tahoma", Font.BOLD, 80));
		btn4.setBounds(10, 10, 132, 164);
		panel_6.add(btn4);
		
		JPanel panel_7 = new JPanel();
		panel_7.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_7);
		panel_7.setLayout(null);
		
		JButton btn5 = new JButton("");
		btn5.setBackground(Color.PINK);
		btn5.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				btn5.setText(startGame);
				if(startGame.equalsIgnoreCase("X"))
				{
					btn5.setForeground(Color.red);
					b5=1;
					i++;
				}
				else
				{
					btn5.setForeground(Color.blue);
					b5=0;
					i++;
				}
				choosePlayer();
				winningGame();
			}
		});
		btn5.setFont(new Font("Tahoma", Font.BOLD, 80));
		btn5.setBounds(10, 10, 132, 164);
		panel_7.add(btn5);
		
		JPanel panel_8 = new JPanel();
		panel_8.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_8);
		panel_8.setLayout(null);
		
		JButton btn6 = new JButton("");
		btn6.setBackground(Color.PINK);
		btn6.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				btn6.setText(startGame);
				if(startGame.equalsIgnoreCase("X"))
				{
					btn6.setForeground(Color.red);
					b6=1;
					i++;
				}
				else
				{
					btn6.setForeground(Color.blue);
					b6=0;
					i++;
				}
				choosePlayer();
				winningGame();
			}
		});
		btn6.setFont(new Font("Tahoma", Font.BOLD, 80));
		btn6.setBounds(10, 10, 132, 164);
		panel_8.add(btn6);
		
		JPanel panel_9 = new JPanel();
		panel_9.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_9);
		panel_9.setLayout(null);
		
		JLabel lblNewLabel_1 = new JLabel("PLAYER O");
		lblNewLabel_1.setBackground(new Color(0, 0, 0));
		lblNewLabel_1.setForeground(Color.MAGENTA);
		lblNewLabel_1.setBounds(10, 10, 132, 164);
		lblNewLabel_1.setHorizontalAlignment(SwingConstants.CENTER);
		lblNewLabel_1.setFont(new Font("Microsoft New Tai Lue", Font.BOLD, 25));
		panel_9.add(lblNewLabel_1);
		
		JPanel panel_10 = new JPanel();
		panel_10.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_10);
		panel_10.setLayout(null);
		
		oCount = new JTextField();
		oCount.setHorizontalAlignment(SwingConstants.CENTER);
		oCount.setBackground(Color.YELLOW);
		oCount.setForeground(Color.BLUE);
		oCount.setFont(new Font("Tw Cen MT Condensed Extra Bold", Font.PLAIN, 45));
		oCount.setText("     0");
		oCount.setBounds(10, 10, 132, 164);
		panel_10.add(oCount);
		oCount.setColumns(10);
		
		JPanel panel_11 = new JPanel();
		panel_11.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_11);
		panel_11.setLayout(null);
		
		JButton btn7 = new JButton("");
		btn7.setBackground(Color.PINK);
		btn7.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				btn7.setText(startGame);
				if(startGame.equalsIgnoreCase("X"))
				{
					btn7.setForeground(Color.red);
					b7=1;
					i++;
				}
				else
				{
					btn7.setForeground(Color.blue);
					b7=0;
					i++;
				}
				choosePlayer();
				winningGame();
			}
		});
		btn7.setFont(new Font("Tahoma", Font.BOLD, 80));
		btn7.setBounds(10, 10, 132, 164);
		panel_11.add(btn7);
		
		JPanel panel_12 = new JPanel();
		panel_12.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_12);
		panel_12.setLayout(null);
		
		JButton btn8 = new JButton("");
		btn8.setBackground(Color.PINK);
		btn8.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				btn8.setText(startGame);
				if(startGame.equalsIgnoreCase("X"))
				{
					btn8.setForeground(Color.red);
					b8=1;
					i++;
				}
				else
				{
					btn8.setForeground(Color.blue);
					b8=0;
					i++;
				}
				choosePlayer();
				winningGame();
			}
		});
		btn8.setFont(new Font("Tahoma", Font.BOLD, 80));
		btn8.setBounds(10, 10, 132, 164);
		panel_12.add(btn8);
		
		JPanel panel_13 = new JPanel();
		panel_13.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_13);
		panel_13.setLayout(null);
		
		JButton btn9 = new JButton("");
		btn9.setBackground(Color.PINK);
		btn9.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				btn9.setText(startGame);
				if(startGame.equalsIgnoreCase("X"))
				{
					btn9.setForeground(Color.red);
					b9=1;
					i++;
				}
				else
				{
					btn9.setForeground(Color.blue);
					b9=0;
					i++;
				}
				choosePlayer();
				winningGame();
			}
		});
		btn9.setFont(new Font("Tahoma", Font.BOLD, 80));
		btn9.setBounds(10, 10, 132, 164);
		panel_13.add(btn9);
		
		JPanel panel_14 = new JPanel();
		panel_14.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_14);
		
		JButton btnReset = new JButton("RESET");
		btnReset.setBackground(Color.GREEN);
		btnReset.setBounds(10, 10, 132, 164);
		btnReset.setFont(new Font("Sitka Small", Font.BOLD, 18));
		btnReset.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				btn1.setText(null);
				btn2.setText(null);
				btn3.setText(null);
				btn4.setText(null);
				btn5.setText(null);
				btn6.setText(null);
				btn7.setText(null);
				btn8.setText(null);
				btn9.setText(null);
				b1=10;
				b2=10;
				b3=10;
				b4=10;
				b5=10;
				b6=10;
				b7=10;
				b8=10;
				b9=10;
				i=0;
			}
		});
		panel_14.setLayout(null);
		panel_14.add(btnReset);
		
		JPanel panel_15 = new JPanel();
		panel_15.setBorder(new LineBorder(new Color(0, 0, 0), 3));
		panel.add(panel_15);
		panel_15.setLayout(null);
		
		JButton btnExit = new JButton("EXIT");
		btnExit.setBackground(Color.RED);
		btnExit.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				
				frame = new JFrame("Exit");
				if(JOptionPane.showConfirmDialog(frame,"ARE YOU SURE, THINK AGAIN","TIC TAC TOE", JOptionPane.YES_NO_OPTION)==JOptionPane.YES_NO_OPTION)
				{
					System.exit(0);
				}
				
			}
		});
		btnExit.setBounds(10, 10, 132, 164);
		btnExit.setFont(new Font("Sitka Small", Font.BOLD, 18));
		panel_15.add(btnExit);
		
		JButton btnTICTACTOE = new JButton("TIC TAC TOE -- GAME FIELD :)");
		 btnTICTACTOE.setBackground(Color.CYAN);
		btnTICTACTOE.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
			}
		});
		btnTICTACTOE.setFont(new Font("Stencil", Font.BOLD, 45));
		btnTICTACTOE.setBounds(0, 567, 776, 170);
		frame.getContentPane().add(btnTICTACTOE);
		
		JButton btnNewButton_1 = new JButton("S");
		btnNewButton_1.setBackground(new Color(255, 69, 0));
		btnNewButton_1.setFont(new Font("Tahoma", Font.BOLD, 35));
		btnNewButton_1.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
			}
		});
		btnNewButton_1.setBounds(781, 10, 85, 32);
		frame.getContentPane().add(btnNewButton_1);
		
		JButton btnNewButton_2 = new JButton("C");
		btnNewButton_2.setBackground(new Color(255, 99, 71));
		btnNewButton_2.setFont(new Font("Tahoma", Font.BOLD, 35));
		btnNewButton_2.setBounds(781, 41, 85, 32);
		frame.getContentPane().add(btnNewButton_2);
		
		JButton btnNewButton_3 = new JButton("O");
		btnNewButton_3.setBackground(new Color(250, 128, 114));
		btnNewButton_3.setFont(new Font("Tahoma", Font.BOLD, 35));
		btnNewButton_3.setBounds(781, 72, 85, 32);
		frame.getContentPane().add(btnNewButton_3);
		
		JButton btnNewButton_4 = new JButton("R");
		btnNewButton_4.setBackground(new Color(255, 160, 122));
		btnNewButton_4.setFont(new Font("Tahoma", Font.BOLD, 35));
		btnNewButton_4.setBounds(781, 104, 85, 32);
		frame.getContentPane().add(btnNewButton_4);
		
		JButton btnNewButton_5 = new JButton("E");
		btnNewButton_5.setBackground(new Color(255, 218, 185));
		btnNewButton_5.setFont(new Font("Tahoma", Font.BOLD, 34));
		btnNewButton_5.setBounds(781, 135, 85, 32);
		frame.getContentPane().add(btnNewButton_5);
		
		JButton btnNewButton_6 = new JButton("B");
		btnNewButton_6.setBackground(new Color(255, 69, 0));
		btnNewButton_6.setFont(new Font("Tahoma", Font.BOLD, 35));
		btnNewButton_6.setBounds(781, 188, 85, 32);
		frame.getContentPane().add(btnNewButton_6);
		
		JButton btnNewButton_7 = new JButton("O");
		btnNewButton_7.setBackground(new Color(255, 99, 71));
		btnNewButton_7.setFont(new Font("Tahoma", Font.BOLD, 35));
		btnNewButton_7.setBounds(781, 219, 85, 32);
		frame.getContentPane().add(btnNewButton_7);
		
		JButton btnNewButton_8 = new JButton("A");
		btnNewButton_8.setBackground(new Color(250, 128, 114));
		btnNewButton_8.setFont(new Font("Tahoma", Font.BOLD, 35));
		btnNewButton_8.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
			}
		});
		btnNewButton_8.setBounds(781, 250, 85, 32);
		frame.getContentPane().add(btnNewButton_8);
		
		JButton btnNewButton_9 = new JButton("R");
		btnNewButton_9.setBackground(new Color(255, 160, 122));
		btnNewButton_9.setFont(new Font("Tahoma", Font.BOLD, 35));
		btnNewButton_9.setBounds(781, 281, 85, 32);
		frame.getContentPane().add(btnNewButton_9);
		
		JButton btnNewButton_10 = new JButton("D");
		btnNewButton_10.setBackground(new Color(255, 222, 173));
		btnNewButton_10.setFont(new Font("Tahoma", Font.BOLD, 35));
		btnNewButton_10.setBounds(781, 313, 85, 38);
		frame.getContentPane().add(btnNewButton_10);
		btnNewButton_3.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
			}
		});
	}
}
