import { motion } from "framer-motion";
import "./index.css";

export default function App() {
  return (
    <div className="container">

      <div className="hero">

        <motion.h1
          initial={{ opacity: 0, y: -40 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 1 }}
        >
          فندق الرويال - عمان
        </motion.h1>

        <motion.p
          initial={{ opacity: 0 }}
          animate={{ opacity: 1 }}
          transition={{ delay: 0.5 }}
        >
          تجربة فاخرة في قلب العاصمة الأردنية
        </motion.p>

        <button className="btn">احجز الآن</button>

      </div>

      <div className="section">
        <h2>عن الفندق</h2>
        <p>
          فندق الرويال يقدم إقامة خمس نجوم، غرف فاخرة، مطاعم عالمية،
          وخدمات راقية في مدينة عمان.
        </p>
      </div>

      <div className="cards">
        <div className="card">غرف فاخرة</div>
        <div className="card">مطاعم</div>
        <div className="card">سبا</div>
      </div>

    </div>
  );
}