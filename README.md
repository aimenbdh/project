# project
mon code 
import java.io.Serializable;
import java.util.List;
import java.util.Map;

/**
 * Cluster info.
 *
 * @author caogu.wyp
 * @version $Id: ClusterInfo.java, v 0.1 2018-09-17 上午11:36 caogu.wyp Exp $$
 */
public class ClusterInfo implements Serializable {
    
    private String clusterName;
    
    private AbstractHealthChecker healthChecker;
    
    private Map<String, String> metadata;
    
    private List<IpAddressInfo> hosts;
    
    /**
     * Getter method for property <tt>hosts</tt>.
     *
     * @return property value of hosts
     */
    public List<IpAddressInfo> getHosts() {
        return hosts;
    }
    
    /**
     * Setter method for property <tt>hosts </tt>.
     *
     * @param hosts value to be assigned to property hosts
     */
    public void setHosts(List<IpAddressInfo> hosts) {
        this.hosts = hosts;
    }
    
    public String getClusterName() {
        return clusterName;
    }
    
    public void setClusterName(String clusterName) {
        this.clusterName = clusterName;
    }
    
    public AbstractHealthChecker getHealthChecker() {
        return healthChecker;
    }
    
    public void setHealthChecker(AbstractHealthChecker healthChecker) {
        this.healthChecker = healthChecker;
    }
    
    public Map<String, String> getMetadata() {
        return metadata;
    }
    
    public void setMetadata(Map<String, String> metadata) {
        this.metadata = metadata;
    }
}
