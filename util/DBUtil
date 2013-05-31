package util;

import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;

/**
 * @author Administrator
 *
 */
public class DBUtil {
  /**
	 * @return
	 */
	public static Connection getConnection(){
		Connection conn = null;
		if(conn==null){
			try {
				Class.forName("com.mysql.jdbc.Driver");
				conn = DriverManager.getConnection(
						"jdbc:mysql://localhost:3306/mbn?useUnicode=true&characterEncoding=utf8",
						"root","");
			} catch (Exception e) {
				e.printStackTrace();
			}
		}
		return conn;
	}
	public static void close(Connection conn){
		if(conn!=null){
			try {
				conn.close();
			} catch (SQLException e) {
				e.printStackTrace();
			}
		}
	}
	
}
